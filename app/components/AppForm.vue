<script setup>
const contactForm = reactive({
  name: "",
  email: "",
  subject: "",
  message: "",
});

const contactErrors = reactive({
  name: "",
  email: "",
  subject: "",
  message: "",
});

const contactFeedback = ref("");

const clearContactFeedback = () => {
  contactFeedback.value = "";
};

const validateContactField = (field) => {
  const value = contactForm[field].trim();

  if (!value) {
    contactErrors[field] = "This field is required.";
    return false;
  }

  if (field === "email") {
    const isValidEmail = /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(value);

    if (!isValidEmail) {
      contactErrors.email = "Enter a valid email address.";
      return false;
    }
  }

  contactErrors[field] = "";
  return true;
};

const validateContactForm = () => {
  return ["name", "email", "subject", "message"].every((field) =>
    validateContactField(field),
  );
};

const handleContactSubmit = () => {
  clearContactFeedback();

  if (validateContactForm()) {
    contactFeedback.value =
      "Form validation passed. Connect this form to your backend or email service to receive submissions.";
    return;
  }

  contactFeedback.value =
    "Please complete the required fields before submitting.";
};
</script>
<template>
  <form
    class="grid grid-cols-2 gap-4 font-normal flex-1"
    novalidate
    @submit.prevent="handleContactSubmit"
  >
    <div class="flex flex-col col-span-2 lg:col-start-1 lg:col-span-1 gap-2">
      <label class="sr-only" for="contact-name">Name</label>
      <input
        id="contact-name"
        v-model="contactForm.name"
        name="name"
        autocomplete="name"
        placeholder="Name"
        class="text-xl p-4 border-2 h-12 lg:h-14"
        :aria-describedby="
          contactErrors.name ? 'contact-name-error' : undefined
        "
        :aria-invalid="contactErrors.name ? 'true' : 'false'"
        required
        type="text"
        @blur="validateContactField('name')"
        @input="
          validateContactField('name');
          clearContactFeedback();
        "
      />
      <p
        v-if="contactErrors.name"
        id="contact-name-error"
        class="text-sm text-red-300"
      >
        {{ contactErrors.name }}
      </p>
    </div>
    <div class="flex flex-col col-span-2 lg:col-span-1 lg:col-start-2 gap-2">
      <label class="sr-only" for="contact-email">Your Email</label>
      <input
        id="contact-email"
        v-model="contactForm.email"
        name="email"
        autocomplete="email"
        placeholder="Your Email"
        class="text-xl p-4 border-2 h-12 lg:h-14"
        :aria-describedby="
          contactErrors.email ? 'contact-email-error' : undefined
        "
        :aria-invalid="contactErrors.email ? 'true' : 'false'"
        required
        type="email"
        @blur="validateContactField('email')"
        @input="
          validateContactField('email');
          clearContactFeedback();
        "
      />
      <p
        v-if="contactErrors.email"
        id="contact-email-error"
        class="text-sm text-red-300"
      >
        {{ contactErrors.email }}
      </p>
    </div>
    <div class="col-span-2 flex flex-col gap-2">
      <label class="sr-only" for="contact-subject">Subject</label>
      <input
        id="contact-subject"
        v-model="contactForm.subject"
        name="subject"
        placeholder="Subject"
        class="text-xl p-4 border-2 col-span-2 h-12 lg:h-14"
        :aria-describedby="
          contactErrors.subject ? 'contact-subject-error' : undefined
        "
        :aria-invalid="contactErrors.subject ? 'true' : 'false'"
        required
        type="text"
        @blur="validateContactField('subject')"
        @input="
          validateContactField('subject');
          clearContactFeedback();
        "
      />
      <p
        v-if="contactErrors.subject"
        id="contact-subject-error"
        class="text-sm text-red-300"
      >
        {{ contactErrors.subject }}
      </p>
    </div>
    <div class="col-span-2 flex flex-col gap-2">
      <label class="sr-only" for="contact-message">Message</label>
      <textarea
        id="contact-message"
        v-model="contactForm.message"
        name="message"
        placeholder="Messages ..."
        class="text-xl p-4 border-2 col-span-2"
        :aria-describedby="
          contactErrors.message ? 'contact-message-error' : undefined
        "
        :aria-invalid="contactErrors.message ? 'true' : 'false'"
        required
        rows="10"
        @blur="validateContactField('message')"
        @input="
          validateContactField('message');
          clearContactFeedback();
        "
      ></textarea>
      <p
        v-if="contactErrors.message"
        id="contact-message-error"
        class="text-sm text-red-300"
      >
        {{ contactErrors.message }}
      </p>
    </div>
    <p v-if="contactFeedback" class="col-span-2 text-sm" aria-live="polite">
      {{ contactFeedback }}
    </p>
    <button
      type="submit"
      class="place-self-end w-30 col-start-2 inline-flex h-12 items-center justify-center border-2 border-white font-semibold text-white transition-colors duration-300 hover:bg-white hover:text-black"
    >
      Reach Me
    </button>
  </form>
</template>
