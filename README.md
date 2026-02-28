<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Privacy Policy — Achieve</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --bg: #f7f5f0;
      --surface: #ffffff;
      --text: #1a1a1a;
      --muted: #6b6b6b;
      --accent: #1a1a1a;
      --border: #e2ddd6;
      --link: #2a52be;
    }

    html { scroll-behavior: smooth; }

    body {
      background: var(--bg);
      color: var(--text);
      font-family: 'DM Sans', sans-serif;
      font-weight: 300;
      line-height: 1.8;
      font-size: 15px;
    }

    /* Header */
    header {
      background: var(--accent);
      color: #fff;
      padding: 0 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 64px;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .logo {
      font-family: 'DM Serif Display', serif;
      font-size: 1.5rem;
      letter-spacing: -0.02em;
      color: #fff;
      text-decoration: none;
    }

    .header-badge {
      font-size: 0.7rem;
      font-weight: 500;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: rgba(255,255,255,0.5);
    }

    /* Hero */
    .hero {
      background: var(--accent);
      color: #fff;
      padding: 5rem 2rem 4rem;
      text-align: center;
      border-bottom: 1px solid #333;
    }

    .hero-label {
      font-size: 0.7rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: rgba(255,255,255,0.45);
      margin-bottom: 1rem;
    }

    .hero h1 {
      font-family: 'DM Serif Display', serif;
      font-size: clamp(2.5rem, 6vw, 4rem);
      line-height: 1.1;
      letter-spacing: -0.02em;
      margin-bottom: 1.25rem;
    }

    .hero-meta {
      color: rgba(255,255,255,0.45);
      font-size: 0.85rem;
    }

    /* Layout */
    .layout {
      max-width: 1100px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 240px 1fr;
      gap: 0;
      padding: 0 2rem;
      align-items: start;
    }

    /* Sidebar TOC */
    .toc {
      position: sticky;
      top: 80px;
      padding: 3rem 2rem 3rem 0;
      border-right: 1px solid var(--border);
    }

    .toc-label {
      font-size: 0.65rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--muted);
      margin-bottom: 1.25rem;
      font-weight: 500;
    }

    .toc ol {
      list-style: none;
      counter-reset: toc;
    }

    .toc ol li {
      counter-increment: toc;
      margin-bottom: 0.35rem;
    }

    .toc ol li a {
      color: var(--muted);
      text-decoration: none;
      font-size: 0.8rem;
      display: flex;
      gap: 0.5rem;
      align-items: baseline;
      transition: color 0.2s;
      line-height: 1.4;
    }

    .toc ol li a::before {
      content: counter(toc, decimal-leading-zero);
      font-size: 0.65rem;
      color: #ccc;
      flex-shrink: 0;
      font-weight: 500;
    }

    .toc ol li a:hover { color: var(--text); }

    /* Main content */
    .content {
      padding: 4rem 0 4rem 3rem;
    }

    .section {
      margin-bottom: 4rem;
      padding-bottom: 4rem;
      border-bottom: 1px solid var(--border);
      opacity: 0;
      transform: translateY(16px);
      animation: fadeUp 0.5s ease forwards;
    }

    .section:last-child { border-bottom: none; }

    @keyframes fadeUp {
      to { opacity: 1; transform: translateY(0); }
    }

    .section:nth-child(1)  { animation-delay: 0.05s; }
    .section:nth-child(2)  { animation-delay: 0.10s; }
    .section:nth-child(3)  { animation-delay: 0.15s; }
    .section:nth-child(4)  { animation-delay: 0.20s; }
    .section:nth-child(5)  { animation-delay: 0.25s; }
    .section:nth-child(6)  { animation-delay: 0.30s; }
    .section:nth-child(7)  { animation-delay: 0.35s; }
    .section:nth-child(8)  { animation-delay: 0.40s; }
    .section:nth-child(9)  { animation-delay: 0.45s; }
    .section:nth-child(10) { animation-delay: 0.50s; }
    .section:nth-child(11) { animation-delay: 0.55s; }
    .section:nth-child(12) { animation-delay: 0.60s; }
    .section:nth-child(13) { animation-delay: 0.65s; }

    .section-number {
      font-size: 0.65rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--muted);
      margin-bottom: 0.5rem;
      font-weight: 500;
    }

    h2 {
      font-family: 'DM Serif Display', serif;
      font-size: 1.6rem;
      line-height: 1.2;
      letter-spacing: -0.01em;
      margin-bottom: 1.5rem;
      color: var(--text);
    }

    h3 {
      font-family: 'DM Sans', sans-serif;
      font-size: 0.9rem;
      font-weight: 500;
      letter-spacing: 0.04em;
      text-transform: uppercase;
      margin: 2rem 0 0.75rem;
      color: var(--text);
    }

    p {
      color: #444;
      margin-bottom: 1rem;
    }

    a { color: var(--link); }

    ul, ol {
      padding-left: 1.5rem;
      margin-bottom: 1rem;
      color: #444;
    }

    li { margin-bottom: 0.4rem; }

    strong { color: var(--text); font-weight: 500; }

    em { font-style: italic; }

    /* Summary callout */
    .summary-box {
      background: var(--bg);
      border: 1px solid var(--border);
      border-left: 3px solid var(--accent);
      padding: 1.5rem;
      margin-bottom: 2rem;
      border-radius: 0 4px 4px 0;
    }

    .summary-box p { margin-bottom: 0.75rem; }
    .summary-box p:last-child { margin-bottom: 0; }

    /* Table */
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 1.5rem 0;
      font-size: 0.875rem;
    }

    th {
      background: var(--bg);
      font-weight: 500;
      text-align: left;
      padding: 0.75rem 1rem;
      border: 1px solid var(--border);
      font-size: 0.75rem;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      color: var(--muted);
    }

    td {
      padding: 0.75rem 1rem;
      border: 1px solid var(--border);
      color: #444;
      vertical-align: middle;
    }

    .yes { color: #1a7a4a; font-weight: 500; }
    .no  { color: var(--muted); }

    /* Contact block */
    .contact-block {
      background: var(--accent);
      color: #fff;
      padding: 2rem;
      border-radius: 4px;
      margin-top: 1.5rem;
    }

    .contact-block p { color: rgba(255,255,255,0.7); margin-bottom: 0.4rem; }
    .contact-block a { color: #fff; }
    .contact-block .contact-name {
      font-family: 'DM Serif Display', serif;
      font-size: 1.2rem;
      color: #fff;
      margin-bottom: 1rem;
    }

    /* Footer */
    footer {
      background: var(--accent);
      color: rgba(255,255,255,0.4);
      text-align: center;
      padding: 2rem;
      font-size: 0.8rem;
      margin-top: 4rem;
    }

    /* Mobile */
    @media (max-width: 768px) {
      .layout { grid-template-columns: 1fr; padding: 0 1.25rem; }
      .toc { display: none; }
      .content { padding: 3rem 0; }
      .hero { padding: 3rem 1.25rem 2.5rem; }
    }
  </style>
</head>
<body>

<header>
  <a class="logo" href="#">Achieve</a>
  <span class="header-badge">Legal</span>
</header>

<div class="hero">
  <p class="hero-label">Legal Document</p>
  <h1>Privacy Policy</h1>
  <p class="hero-meta">Last updated February 28, 2026</p>
</div>

<div class="layout">

  <!-- Sidebar TOC -->
  <nav class="toc">
    <p class="toc-label">Contents</p>
    <ol>
      <li><a href="#s1">What Information Do We Collect?</a></li>
      <li><a href="#s2">How Do We Process Your Information?</a></li>
      <li><a href="#s3">Legal Bases for Processing</a></li>
      <li><a href="#s4">When Do We Share Information?</a></li>
      <li><a href="#s5">AI-Based Products</a></li>
      <li><a href="#s6">How Long Do We Keep Info?</a></li>
      <li><a href="#s7">How Do We Keep Info Safe?</a></li>
      <li><a href="#s8">Your Privacy Rights</a></li>
      <li><a href="#s9">Do-Not-Track Controls</a></li>
      <li><a href="#s10">US Residents' Rights</a></li>
      <li><a href="#s11">Updates to This Notice</a></li>
      <li><a href="#s12">How to Contact Us</a></li>
      <li><a href="#s13">Review or Delete Your Data</a></li>
    </ol>
  </nav>

  <!-- Main Content -->
  <main class="content">

    <!-- Intro -->
    <div class="section" id="intro">
      <p>This Privacy Notice for <strong>Achieve</strong> ("we," "us," or "our") describes how and why we might access, collect, store, use, and/or share ("process") your personal information when you use our services, including when you:</p>
      <ul>
        <li>Visit our website at <a href="http://achi3ve.ca/" target="_blank">http://achi3ve.ca/</a> or any website of ours that links to this Privacy Notice</li>
        <li>Engage with us in other related ways, including any marketing or events</li>
      </ul>
      <p><strong>Questions or concerns?</strong> Reading this Privacy Notice will help you understand your privacy rights and choices. If you do not agree with our policies and practices, please do not use our Services. If you still have any questions or concerns, please contact us at <a href="mailto:zane.rw.robertson@gmail.com">zane.rw.robertson@gmail.com</a>.</p>
    </div>

    <!-- Summary -->
    <div class="section" id="summary">
      <p class="section-number">Summary</p>
      <h2>Key Points</h2>
      <div class="summary-box">
        <p><strong>What personal information do we process?</strong> When you visit, use, or navigate our Services, we may process personal information depending on how you interact with us and the Services, the choices you make, and the products and features you use.</p>
        <p><strong>Do we process any sensitive personal information?</strong> We may process sensitive personal information when necessary with your consent or as otherwise permitted by applicable law.</p>
        <p><strong>Do we collect any information from third parties?</strong> We do not collect any information from third parties.</p>
        <p><strong>How do we process your information?</strong> We process your information to provide, improve, and administer our Services, communicate with you, for security and fraud prevention, and to comply with law.</p>
        <p><strong>In what situations and with which parties do we share personal information?</strong> We may share information in specific situations and with specific third parties.</p>
        <p><strong>How do we keep your information safe?</strong> We have adequate organizational and technical processes in place to protect your personal information. However, no electronic transmission over the internet can be guaranteed to be 100% secure.</p>
        <p><strong>What are your rights?</strong> Depending on where you are located geographically, you may have certain rights regarding your personal information.</p>
        <p><strong>How do you exercise your rights?</strong> The easiest way to exercise your rights is by submitting a <a href="https://app.termly.io/dsar/74a07e1b-3c05-45c6-8435-e95de1d9f1e0" target="_blank">data subject access request</a>, or by contacting us.</p>
      </div>
    </div>

    <!-- Section 1 -->
    <div class="section" id="s1">
      <p class="section-number">01</p>
      <h2>What Information Do We Collect?</h2>
      <h3>Personal Information You Disclose to Us</h3>
      <p>We collect personal information that you voluntarily provide to us when you express an interest in obtaining information about us or our products and Services, when you participate in activities on the Services, or otherwise when you contact us.</p>
      <p><strong>Personal Information Provided by You.</strong> The personal information we collect may include: names, phone numbers, email addresses, contact preferences, contact or authentication data, debit/credit card numbers, billing addresses, mailing addresses, job titles, usernames, and passwords.</p>
      <h3>Sensitive Information</h3>
      <p>When necessary, with your consent or as otherwise permitted by applicable law, we process the following categories of sensitive information: financial data, health data, genetic data, biometric data, data about a person's sex life or sexual orientation, information revealing race or ethnic origin, information revealing trade union membership, and student data.</p>
      <p>All personal information that you provide to us must be true, complete, and accurate, and you must notify us of any changes to such personal information.</p>
      <h3>Google API</h3>
      <p>Our use of information received from Google APIs will adhere to the <a href="https://developers.google.com/terms/api-services-user-data-policy" target="_blank">Google API Services User Data Policy</a>, including the <a href="https://developers.google.com/terms/api-services-user-data-policy#limited-use" target="_blank">Limited Use requirements</a>.</p>
    </div>

    <!-- Section 2 -->
    <div class="section" id="s2">
      <p class="section-number">02</p>
      <h2>How Do We Process Your Information?</h2>
      <p><em><strong>In Short:</strong> We process your information to provide, improve, and administer our Services, communicate with you, for security and fraud prevention, and to comply with law.</em></p>
      <p>We process your personal information for a variety of reasons, depending on how you interact with our Services, including:</p>
      <ul>
        <li><strong>To deliver and facilitate delivery of services to the user.</strong> We may process your information to provide you with the requested service.</li>
        <li><strong>To fulfill and manage your orders.</strong> We may process your information to fulfill and manage your orders, payments, returns, and exchanges made through the Services.</li>
        <li><strong>To enable user-to-user communications.</strong> We may process your information if you choose to use any of our offerings that allow for communication with another user.</li>
        <li><strong>To request feedback.</strong> We may process your information when necessary to request feedback and to contact you about your use of our Services.</li>
        <li><strong>To post testimonials.</strong> We post testimonials on our Services that may contain personal information.</li>
        <li><strong>To protect our Services.</strong> We may process your information as part of our efforts to keep our Services safe and secure, including fraud monitoring and prevention.</li>
        <li><strong>To evaluate and improve our Services, products, marketing, and your experience.</strong> We may process your information when we believe it is necessary to identify usage trends, determine the effectiveness of our promotional campaigns, and to evaluate and improve our Services, products, marketing, and your experience.</li>
        <li><strong>To identify usage trends.</strong> We may process information about how you use our Services to better understand how they are being used so we can improve them.</li>
      </ul>
    </div>

    <!-- Section 3 -->
    <div class="section" id="s3">
      <p class="section-number">03</p>
      <h2>What Legal Bases Do We Rely On to Process Your Information?</h2>
      <p><em><strong>In Short:</strong> We only process your personal information when we believe it is necessary and we have a valid legal reason to do so under applicable law.</em></p>
      <p><strong><u>If you are located in Canada, this section applies to you.</u></strong></p>
      <p>We may process your information if you have given us specific permission (express consent) to use your personal information for a specific purpose, or in situations where your permission can be inferred (implied consent). You can withdraw your consent at any time.</p>
      <p>In some exceptional cases, we may be legally permitted under applicable law to process your information without your consent, including:</p>
      <ul>
        <li>If collection is clearly in the interests of an individual and consent cannot be obtained in a timely way</li>
        <li>For investigations and fraud detection and prevention</li>
        <li>For business transactions provided certain conditions are met</li>
        <li>If it is contained in a witness statement and the collection is necessary to assess, process, or settle an insurance claim</li>
        <li>For identifying injured, ill, or deceased persons and communicating with next of kin</li>
        <li>If we have reasonable grounds to believe an individual has been, is, or may be victim of financial abuse</li>
        <li>If disclosure is required to comply with a subpoena, warrant, court order, or rules of the court relating to the production of records</li>
        <li>If it was produced by an individual in the course of their employment, business, or profession and the collection is consistent with the purposes for which the information was produced</li>
        <li>If the collection is solely for journalistic, artistic, or literary purposes</li>
        <li>If the information is publicly available and is specified by the regulations</li>
        <li>We may disclose de-identified information for approved research or statistics projects, subject to ethics oversight and confidentiality commitments</li>
      </ul>
    </div>

    <!-- Section 4 -->
    <div class="section" id="s4">
      <p class="section-number">04</p>
      <h2>When and With Whom Do We Share Your Personal Information?</h2>
      <p><em><strong>In Short:</strong> We may share information in specific situations described in this section and/or with the following third parties.</em></p>
      <p>We may need to share your personal information in the following situations:</p>
      <ul>
        <li><strong>Business Transfers.</strong> We may share or transfer your information in connection with, or during negotiations of, any merger, sale of company assets, financing, or acquisition of all or a portion of our business to another company.</li>
      </ul>
    </div>

    <!-- Section 5 -->
    <div class="section" id="s5">
      <p class="section-number">05</p>
      <h2>Do We Offer Artificial Intelligence-Based Products?</h2>
      <p><em><strong>In Short:</strong> We offer products, features, or tools powered by artificial intelligence, machine learning, or similar technologies.</em></p>
      <p>As part of our Services, we offer products, features, or tools powered by artificial intelligence, machine learning, or similar technologies (collectively, "AI Products"). These tools are designed to enhance your experience and provide you with innovative solutions. The terms in this Privacy Notice govern your use of the AI Products within our Services.</p>
      <h3>Use of AI Technologies</h3>
      <p>We provide the AI Products through third-party service providers ("AI Service Providers"), including <strong>OpenAI</strong>. Your input, output, and personal information will be shared with and processed by these AI Service Providers to enable your use of our AI Products. You must not use the AI Products in any way that violates the terms or policies of any AI Service Provider.</p>
      <h3>Our AI Products</h3>
      <p>Our AI Products are designed for the following functions: AI automation.</p>
      <h3>How We Process Your Data Using AI</h3>
      <p>All personal information processed using our AI Products is handled in line with our Privacy Notice and our agreement with third parties. This ensures high security and safeguards your personal information throughout the process.</p>
    </div>

    <!-- Section 6 -->
    <div class="section" id="s6">
      <p class="section-number">06</p>
      <h2>How Long Do We Keep Your Information?</h2>
      <p><em><strong>In Short:</strong> We keep your information for as long as necessary to fulfill the purposes outlined in this Privacy Notice unless otherwise required by law.</em></p>
      <p>We will only keep your personal information for as long as it is necessary for the purposes set out in this Privacy Notice, unless a longer retention period is required or permitted by law (such as tax, accounting, or other legal requirements).</p>
      <p>When we have no ongoing legitimate business need to process your personal information, we will either delete or anonymize such information, or, if this is not possible (for example, because your personal information has been stored in backup archives), then we will securely store your personal information and isolate it from any further processing until deletion is possible.</p>
    </div>

    <!-- Section 7 -->
    <div class="section" id="s7">
      <p class="section-number">07</p>
      <h2>How Do We Keep Your Information Safe?</h2>
      <p><em><strong>In Short:</strong> We aim to protect your personal information through a system of organizational and technical security measures.</em></p>
      <p>We have implemented appropriate and reasonable technical and organizational security measures designed to protect the security of any personal information we process. However, despite our safeguards and efforts to secure your information, no electronic transmission over the Internet or information storage technology can be guaranteed to be 100% secure, so we cannot promise or guarantee that hackers, cybercriminals, or other unauthorized third parties will not be able to defeat our security and improperly collect, access, steal, or modify your information. Although we will do our best to protect your personal information, transmission of personal information to and from our Services is at your own risk. You should only access the Services within a secure environment.</p>
    </div>

    <!-- Section 8 -->
    <div class="section" id="s8">
      <p class="section-number">08</p>
      <h2>What Are Your Privacy Rights?</h2>
      <p><em><strong>In Short:</strong> Depending on your state of residence in the US or in some regions, such as Canada, you have rights that allow you greater access to and control over your personal information.</em></p>
      <p>In some regions (like Canada), you have certain rights under applicable data protection laws. These may include the right (i) to request access and obtain a copy of your personal information, (ii) to request rectification or erasure; (iii) to restrict the processing of your personal information; (iv) if applicable, to data portability; and (v) not to be subject to automated decision-making.</p>
      <p>In certain circumstances, you may also have the right to object to the processing of your personal information. You can make such a request by contacting us using the contact details provided in the section "HOW CAN YOU CONTACT US ABOUT THIS NOTICE?" below.</p>
      <h3>Withdrawing Your Consent</h3>
      <p>If we are relying on your consent to process your personal information, you have the right to withdraw your consent at any time by contacting us using the contact details provided below.</p>
      <h3>Opting Out of Marketing</h3>
      <p>You can unsubscribe from our marketing and promotional communications at any time by replying "STOP" or "UNSUBSCRIBE" to the SMS messages that we send, or by contacting us using the details provided below.</p>
      <p><strong>No mobile information will be shared with third parties or affiliates for marketing or promotional purposes.</strong> Information sharing to subcontractors in support services, such as customer service, is permitted. All other use case categories exclude text messaging originator opt-in data and consent; this information will not be shared with third parties.</p>
      <p>If you have questions or comments about your privacy rights, you may email us at <a href="mailto:zane.rw.robertson@gmail.com">zane.rw.robertson@gmail.com</a>.</p>
    </div>

    <!-- Section 9 -->
    <div class="section" id="s9">
      <p class="section-number">09</p>
      <h2>Controls for Do-Not-Track Features</h2>
      <p>Most web browsers and some mobile operating systems and mobile applications include a Do-Not-Track ("DNT") feature or setting you can activate to signal your privacy preference not to have data about your online browsing activities monitored and collected. At this stage, no uniform technology standard for recognizing and implementing DNT signals has been finalized. As such, we do not currently respond to DNT browser signals or any other mechanism that automatically communicates your choice not to be tracked online. If a standard for online tracking is adopted that we must follow in the future, we will inform you about that practice in a revised version of this Privacy Notice.</p>
      <p>California law requires us to let you know how we respond to web browser DNT signals. Because there currently is not an industry or legal standard for recognizing or honoring DNT signals, we do not respond to them at this time.</p>
    </div>

    <!-- Section 10 -->
    <div class="section" id="s10">
      <p class="section-number">10</p>
      <h2>Do United States Residents Have Specific Privacy Rights?</h2>
      <p><em><strong>In Short:</strong> If you are a resident of California, Colorado, Connecticut, Delaware, Florida, Indiana, Iowa, Kentucky, Maryland, Minnesota, Montana, Nebraska, New Hampshire, New Jersey, Oregon, Rhode Island, Tennessee, Texas, Utah, or Virginia, you may have the right to request access to and receive details about the personal information we maintain about you.</em></p>
      <h3>Categories of Personal Information We Collect</h3>
      <table>
        <thead>
          <tr>
            <th>Category</th>
            <th>Examples</th>
            <th>Collected</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>A. Identifiers</td><td>Contact details, name, email, IP address, account name</td><td class="no">NO</td></tr>
          <tr><td>B. Personal info (California Customer Records statute)</td><td>Name, contact information, education, employment, financial information</td><td class="no">NO</td></tr>
          <tr><td>C. Protected classification characteristics</td><td>Gender, age, race, national origin, marital status</td><td class="no">NO</td></tr>
          <tr><td>D. Commercial information</td><td>Transaction information, purchase history, financial details</td><td class="no">NO</td></tr>
          <tr><td>E. Biometric information</td><td>Fingerprints and voiceprints</td><td class="no">NO</td></tr>
          <tr><td>F. Internet or network activity</td><td>Browsing history, search history, online behavior</td><td class="no">NO</td></tr>
          <tr><td>G. Geolocation data</td><td>Device location</td><td class="no">NO</td></tr>
          <tr><td>H. Audio, electronic, or similar information</td><td>Images and audio, video or call recordings</td><td class="no">NO</td></tr>
          <tr><td>I. Professional or employment-related information</td><td>Business contact details, work history, professional qualifications</td><td class="no">NO</td></tr>
          <tr><td>J. Education information</td><td>Student records and directory information</td><td class="no">NO</td></tr>
          <tr><td>K. Inferences from collected information</td><td>Inferences to create a profile about preferences and characteristics</td><td class="no">NO</td></tr>
          <tr><td>L. Sensitive personal information</td><td>Biometric data, account login, debit/credit card numbers, health data, genetic data, racial or ethnic origin</td><td class="yes">YES</td></tr>
        </tbody>
      </table>
      <p>We only collect sensitive personal information, as defined by applicable privacy laws or the purposes allowed by law or with your consent.</p>
      <h3>Your Rights</h3>
      <p>You have rights under certain US state data protection laws. These rights include: right to know, right to access, right to correct inaccuracies, right to request deletion, right to obtain a copy, right to non-discrimination, and right to opt out of the sale of personal data or profiling.</p>
      <h3>How to Exercise Your Rights</h3>
      <p>To exercise these rights, you can contact us by submitting a <a href="https://app.termly.io/dsar/74a07e1b-3c05-45c6-8435-e95de1d9f1e0" target="_blank">data subject access request</a>, by emailing us at <a href="mailto:zane.rw.robertson@gmail.com">zane.rw.robertson@gmail.com</a>, or by calling toll-free at 416-660-3723.</p>
      <h3>Appeals</h3>
      <p>Under certain US state data protection laws, if we decline to take action regarding your request, you may appeal our decision by emailing us at <a href="mailto:zane.rw.robertson@gmail.com">zane.rw.robertson@gmail.com</a>. If your appeal is denied, you may submit a complaint to your state attorney general.</p>
    </div>

    <!-- Section 11 -->
    <div class="section" id="s11">
      <p class="section-number">11</p>
      <h2>Do We Make Updates to This Notice?</h2>
      <p><em><strong>In Short:</strong> Yes, we will update this notice as necessary to stay compliant with relevant laws.</em></p>
      <p>We may update this Privacy Notice from time to time. The updated version will be indicated by an updated "Revised" date at the top of this Privacy Notice. If we make material changes to this Privacy Notice, we may notify you either by prominently posting a notice of such changes or by directly sending you a notification. We encourage you to review this Privacy Notice frequently to be informed of how we are protecting your information.</p>
    </div>

    <!-- Section 12 -->
    <div class="section" id="s12">
      <p class="section-number">12</p>
      <h2>How Can You Contact Us About This Notice?</h2>
      <p>If you have questions or comments about this notice, you may email us at <a href="mailto:zane.rw.robertson@gmail.com">zane.rw.robertson@gmail.com</a> or contact us by post at:</p>
      <div class="contact-block">
        <p class="contact-name">Achieve</p>
        <p>237 Sawmill Valley Drive</p>
        <p>Newmarket, Ontario L3X 2W4</p>
        <p>Canada</p>
        <p style="margin-top:1rem;"><a href="mailto:zane.rw.robertson@gmail.com">zane.rw.robertson@gmail.com</a></p>
        <p>416-660-3723</p>
      </div>
    </div>

    <!-- Section 13 -->
    <div class="section" id="s13">
      <p class="section-number">13</p>
      <h2>How Can You Review, Update, or Delete the Data We Collect From You?</h2>
      <p>Based on the applicable laws of your country or state of residence in the US, you may have the right to request access to the personal information we collect from you, details about how we have processed it, correct inaccuracies, or delete your personal information. You may also have the right to withdraw your consent to our processing of your personal information.</p>
      <p>To request to review, update, or delete your personal information, please fill out and submit a <a href="https://app.termly.io/dsar/74a07e1b-3c05-45c6-8435-e95de1d9f1e0" target="_blank">data subject access request</a>.</p>
    </div>

  </main>
</div>

<footer>
  <p>© 2026 Achieve. Privacy policy generated with Termly.</p>
</footer>

</body>
</html>
