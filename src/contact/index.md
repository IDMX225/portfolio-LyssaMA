---
layout: base.njk
title: Contact
permalink: /contact/
---

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ title }}</title>

  <!-- Favicon -->
  <link rel="icon" href="assets/TP GOLD TRIM (4K x 4K).svg" type="image/svg+xml">
  <!-- for older browser support -->
  <link rel="icon" href="images/TP GOLD TRIM (4K x 4K).png" sizes="32x32" type="image/png">

  <style>
    /* General Form Styles */
    form {
      max-width: 700px;
      margin: 0 auto;
      padding: 20px;
      background-color: #f9f9f9;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    /* Label Styles */
    label {
      display: block;
      margin-bottom: 5px;
      font-weight: bold;
      color: #333;
    }

    /* Input Fields */
    input[type="text"],
    input[type="email"],
    textarea {
      width: 100%;
      padding: 20px;
      margin-bottom: 15px;
      border: 1px solid #ddd;
      border-radius: 4px;
      font-size: 16px;
      color: #333;
    }

    /* Textarea Styling */
    textarea {
      resize: vertical;
      height: 150px;
    }

    /* Submit Button */
    button {
      padding: 12px 20px;
      background-color: #b26834; /* Saddle Brown */
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    /* Button Hover Effect */
    button:hover {
      background-color: #3b2e2e; /* Dark Brown */
    }

    /* Error Message Style */
    .error {
      color: red;
      font-size: 14px;
      margin-top: 10px;
    }

    /* Section Title */
    .section-title {
      text-align: center;
      font-size: 3rem;
      color: #1e1e1e; /* Dark Brown */
    }

    /* Contact Button Container */
    .contact-button-container {
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }

    /* Contact Button Styling */
    .contact-button {
      padding: 12px 20px;
      background-color: #b26834; /* Saddle Brown */
      color: white;
      font-size: 18px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      text-decoration: none;
      transition: background-color 0.3s ease;
    }

    /* Contact Button Hover Effect */
    .contact-button:hover {
      background-color: #3b2e2e; /* Dark Brown */
    }

    /* Form Button Container */
    .form-btn-container {
      text-align: center;
    }

    /* Responsive Form Styles */
    @media (max-width: 768px) {
      form {
        padding: 15px;
      }

      .contact-button,
      button {
        width: 100%;
        padding: 14px 20px;
      }
    }

    /* Logo for contact page */
    .contact-logo-container {
      text-align: center;
      margin-bottom: 20px;
    }

    .contact-logo {
      width: 120px; 
      height: auto;
    }
  </style>
</head>

<section class="contact">
  <div class="container flow">
    <div class="contact-logo-container">
      <img src="/images/TP GOLD TRIM (4K x 4K).png" alt="True Poet Digital Designs Logo" class="contact-logo">
    </div>
    
    <!-- Header title -->
    <h2 class="section-title">Contact Us</h2>
    
    <form name="contact" method="POST" data-netlify="true" id="contact-form">
      <input type="hidden" name="form-name" value="contact">
      
      <p>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
      </p>
      <p>
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
      </p>
      <p>
        <label for="message">Message:</label>
        <textarea id="message" name="message" required></textarea>
      </p>
      
      <!-- Send Button -->
      <div class="form-btn-container">
        <button type="submit">Send</button>
      </div>
    </form>
  </div>
</section>
