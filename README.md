# LSA-Email-Template-Full
This is the single-column email communication template provided by the College of Literature, Science and the Arts department of Marketing and Communications. This template is designed and developed by the department of Marketing and Communications and leverages the [Cerberus fluid email template](https://tedgoas.github.io/Cerberus/). The template is fluid -- not responsive. In other words, the content will scale down for smaller devices but will not reorder or reposition.

This file requires some basic HTML knowledge in order to use. At the very least, you will need to provide a header image, footer image, and body copy in the HTML code.

Images are currently local references. If you want to load the image from a CDN (our web drive, for example) you will need to provide the proper image href properties.

For design guidelines, refer to the [Style Guide](#style-guide). **Any components not included in this template will require custom development. Please work with the developer and project manager to plan for this prior to designing**.

View a preview of the template here: **[Template Preview](http://webapps.lsa.umich.edu/project/lsa-email/LSA-Email-Template/LSA-Email-Communication-Template-V1-0.html)**

## Table of Contents
1. **[Features](#features)**
2. [**How To Use**](#how-to-use)
3. [**Style Guide**](#style-guide)
    1. [**Color**](#color)
    2. [**Typography**](#typography)
    3. 




## Features
- Single-column layout.
- 600px width fluid design. Will resize content on screens smaller than 600px.
- Header and footer placeholder.
- Fully commented code.
- Component driven design. Copy and paste provided code blocks to add different components.

## How to Use
1. Click the green **Clone or Download** button and select the **Download ZIP** button.
2. Change the header image.
3. Change the footer image.
4. Change the body copy.
5. (optional) Change the [Preview Text](#visually-hidden-preview-text)
5. If you're using Campaign Monitor
- Use this footer code to include the unsubscribe

```
<!-- Unsubscribe Footer : BEGIN -->
      <table align="center" role="presentation" cellspacing="0" cellpadding="0" border="0" width="100%" style="margin: auto;">
        <tr>
          <td style="padding: 20px; font-family: sans-serif; font-size: 12px; line-height: 15px; text-align: center; color: #888888;">
            <unsubscribe style="color: #cccccc; text-decoration: underline; font-weight: bold;">Unsubscribe</unsubscribe>
            &nbsp;&nbsp;|&nbsp;&nbsp;
            <webversion style="color: #cccccc; text-decoration: underline; font-weight: bold;">View as a Web Page</webversion>
            <br>
            <br>
          </td>
        </tr>
      </table>
<!-- Unsubscribe Footer : END -->
```

## Style Guide
### Color
All colors should use the approved [LSA color palette](https://codepen.io/joshsalazar/pen/ZVLqrR).

The background is UMich Blue (#00274C).

Links are LSA Cyan (#007CBA), dotted, and underlined.

Body copy is Web Grey 1 (#333333).

Button backgrounds are LSA cyan (#007CBA) with white (#FFFFFF) text. Refer to the [Button](#button) component for HTML and CSS component code reference.

### Typography
Body copy is the serif font Georgia with a minimum of 16px. Line height (leading) should be 24px. Refer to the [Paragraphs](#paragraphs) section for HTML and CSS component code reference.

> *Accessibility* - For Accessibility, body copy needs to be at least 16px high with a line-height (leading) of 24px.

Salutations are 18px, bold, and italicized. Refer to the [Salutations](#salutations) component for HTML and CSS component code reference.

Buttons are 15px, Georgia serif. Refer to the [Button](#button) component for HTML and CSS component code reference.

### Iconography
The use of text character emojis is allowed in HTML emails. To access the list of available text-based emojis, press `cmd+ctrl+space` (Apple) or `Windows+semi-colon` (PC).

> *Accessibility* - For Accessibility do not use emojis alone to convey information. Ask yourself "if this emoji didn't exist, is the purpose of the message still getting through?" If not, don't use an emoji. Emojis add flavor. A bad example of using an emoji would be "Welcome to the new LSA 🏛!" where the building emoji is replacing the word "building. A good example of using an emoji would be "Welcome to the new LSA Building 🏛!"

### Motion
HTML emails support .gif image format. View this [live example](http://webapps.lsa.umich.edu/project/lsa-email/2020/200028G-LSA-Building-Opening-Email/[TEST%203]%20200028G-LSA-Building-Opening-Email.html) of a .gif animation in a header.

.gifs are best if subtle and not overused.

## Components

### Button
There should only be one button in the email. This button should be the primary call to action.

Buttons have a 4px border-radius, line-height of 15px, font-size of 15px, and padding of 13px top/bottom 17px left/right.
```
<!-- Button : BEGIN -->
<tr>
   <td style="padding: 20px 20px">
      <table align="center" role="presentation" cellspacing="0" cellpadding="0" border="0" style="margin: auto;">
         <tr>
            <td class="button-td button-td-primary" style="border-radius: 4px; background: #007CBA;">
               <a class="button-a button-a-primary" href="https://google.com/" style="background: #007CBA; font-family: Georgia, Garamond, Times New Roman, Times, serif; font-size: 15px; line-height: 15px; text-decoration: none; padding: 13px 17px; color: #ffffff; display: block; border-radius: 4px;">
               </a>
            </td>
         </tr>
      </table>
   </td>
</tr>
<!-- Button : END -->
```

### Paragraphs
```
<!-- Paragraphs : BEGIN -->
<tr>
  <td style="padding: 20px; font-family: Georgia, Garamond, Times New Roman, Times, serif; font-size: 16px; line-height: 24px; color: #333333;">
    <p style="margin: 0;">
      <strong style="font-family: Georgia, Garamond, Times New Roman, Times, serif; font-size: 18px; line-height:24px;"><em>Greetings,</em></strong>
      <br />
      <br />
      This is <strong>version 1.0</strong> of the fluid email template provided by the College of Literature, Science, and the Arts Marketing and Communications department. This template is intended for single-column email
                    communications. This template is not designed to leverage multiple columns.
      <br />
      <br />
      Each paragraph should be broken up by two linebreak tags. <a href="#" style="color: #007CBA; text-decoration: none; border-bottom: dotted; border-width: 1px; border-color: #007CBA;">Links</a> should look like this. You can use the email href property to link emails like this <a style="color: #007CBA; text-decoration: none; border-bottom: dotted; border-width: 1px; border-color: #007CBA;" href="mailto: lsa@umich.edu">lsa@umich.edu</a> and the tel property to link telephone numbers <a style="color: #007CBA; text-decoration: none; border-bottom: dotted; border-width: 1px; border-color: #007CBA;" href="tel:7349369999">734.936.9999</a>.
    </p>
  </td>
</tr>
<!-- Paragraphs : END -->
```

#### Salutations
Salutations live in a Paragraph component (as seen above) but are bolded, 18px, and italicized.
```
<strong style="font-family: Georgia, Garamond, Times New Roman, Times, serif; font-size: 18px; line-height:24px;"><em>Greetings,</em></strong>
```

### Visually Hidden Preview Text
Preview text is a snippet of copy pulled in from the body of your email and typically displayed underneath the sender name and subject line in a subscriber’s inbox.

The concept of preview text is reminiscent of the “Johnson Box” used on direct mail pieces to draw readers’ attention to key points of a message. The same goal applies to email—preview text can capture your subscriber’s attention, encouraging them to open. Preview text can also influence behavior—getting subscribers to scroll and click specific articles mentioned in the text.

Email clients will generally pull the first bit of text from the email and display that as the preview text. This code forces the client to display this text as the preview and allows the campaign to have more specific messaging.

Though this code technically lives in the HTML, it is coded in such a way that recipients won't be able to see it when they open the email. It will only display in the inbox preview.
```
<!-- Visually Hidden Preview Text : BEGIN -->
<div style="display: none; font-size: 1px; line-height: 1px; max-height: 0px; max-width: 0px; opacity: 0; overflow: hidden; mso-hide: all; font-family: sans-serif;">
      (Optional) This text will appear in the inbox preview, but not the email body. It can be used to supplement the email subject line or even summarize the email's contents. Extended text preheaders (~490 characters) seems like a better UX for
      anyone using a screenreader or voice-command apps like Siri to dictate the contents of an email. If this text is not included, email clients will automatically populate it using the text (including image alt text) at the start of the email's
      body.
</div>
<!-- Visually Hidden Preview Text : END -->

<!-- Preview Text Spacing : BEGIN -->
<div style="display: none; font-size: 1px; line-height: 1px; max-height: 0px; max-width: 0px; opacity: 0; overflow: hidden; mso-hide: all; font-family: sans-serif;">
      &zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;&zwnj;&nbsp;
</div>
<!-- Preview Text Spacing : END -->
```

### Full-Width Image

```
<!-- Full-width Image : BEGIN -->
<tr>
  <td style="padding: 0 20px; font-family: Georgia, Garamond, Times New Roman, Times, serif; font-size: 16px; line-height: 22px; color: #333333;">
    <img src="images/full-width-image.png" width="600" height="auto" alt="Dean Anne Curzan in a library, overlay text reads Happy Holidays."
                      border="0" style="width: 100%; max-width: 600px; height: auto; background: #dddddd; font-family: sans-serif; font-size: 16px; line-height: 15px; color: #555555; display: block; margin-bottom: 20px;" class="g-img">
  </td>
</tr>
<!-- Full-width Image : END -->
```

### Header Image
The header image is constrained to 600px wide. It is recommended the image itself is 1000px - 1200px wide. This makes the image more crsip once scaled down to 600px.

The height of the image does not matter.

```
<tr>
  <td style="background-color: #ffffff;">
    <img src="images/header-placeholder-200px.png" width="600" height="" alt="alt_text" border="0" style="width: 100%; max-width: 600px; height: auto; background: #dddddd; font-family: sans-serif; font-size: 16px; line-height: 15px; color: #555555; margin: auto; display: block;" class="g-img">
  </td>
</tr>
```

### Footer Image
The header image is constrained to 600px wide. It is recommended the image itself is 1000px - 1200px wide. This makes the image more crsip once scaled down to 600px.
```
<!-- Footer Image, Flush : BEGIN -->
<tr>
  <td style="background-color: #ffffff;">
    <img src="images/footer-placeholder.png" width="600" height="" alt="alt_text" border="0" style="width: 100%; max-width: 600px; height: auto; background: #dddddd; font-family: sans-serif; font-size: 15px; line-height: 15px; color: #555555; margin: auto; display: block;" class="g-img">
  </td>
</tr>
<!-- Footer Image, Flush : END -->
```

## Changelog
### v1.0
- Initial file creation. Modified Cerberus fluid email template to coincide with LSA marketing and branding standards. Inbox tested and fully vetted.


