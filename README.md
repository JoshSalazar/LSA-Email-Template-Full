# LSA-Email-Template-Full
This is the single-column email communication template provided by the College of Literature, Science and the Arts department of Marketing and Communications. This template is designed and developed by the department of Marketing and Communications and leverages the [Cerberus fluid email template](https://tedgoas.github.io/Cerberus/).

This file requires some basic HTML knowledge in order to use. At the very least, you will need to provide a header image, footer image, and body copy in the HTML code.

Images are currently local references. If you want to load the image from a CDN (our web drive, for example) you will need to provide the proper image href properties.

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

6. If you're using Mail Chimp
- Test

### OPTIONAL
- Add hidden preview text. This text will show up after the subject line in the inbox. It's a good place to add teaser text to encourage the recipient to open the email. 

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

## Components
Button: There should only be one button in the email. This button should be the primary call to action.
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

## Changelog
### v1.0
- Initial file creation. Modified Cerberus fluid email template to coincide with LSA marketing and branding standards. Inbox tested and fully vetted.


