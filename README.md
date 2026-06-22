# Common Room Identify Tag for Google Tag Manager

A Google Tag Manager Custom Tag Template for identifying authenticated users in Common Room using the Common Room Signals API.

This template allows GTM users to send user identity information to Common Room using an email address and an optional name value.

## Features

* Identify authenticated users in Common Room
* Supports dynamic GTM variables
* Email field required
* Name field optional
* Optional debug logging
* Simple GTM configuration
* Community Template Gallery ready

## Requirements

Before using this template, ensure that Common Room Signals has already been installed on your website.

Official Common Room Signals documentation:

https://www.commonroom.io/docs/signals/website-visitor-tracking/

## Template Fields

| Field                | Required | Description                                                             |
| -------------------- | -------- | ----------------------------------------------------------------------- |
| Email                | Yes      | Email address used to identify the visitor in Common Room.              |
| Name                 | No       | Visitor name to associate with the identified profile.                  |
| Enable Debug Logging | No       | Enables diagnostic messages in the browser console for troubleshooting. |

## How It Works

When the tag fires, the template sends an identify request to Common Room using the values provided in the template fields.

The Email field is required because Common Room uses the email address to identify and associate visitor activity with a known profile.

The Name field is optional and can be used to enrich the profile when available.

## Example Configuration

| Field                | Example Value                                  |
| -------------------- | ---------------------------------------------- |
| Email                | {{User Email}}                                 |
| Name                 | {{User Full Name}}                             |
| Enable Debug Logging | Enabled during testing, disabled in production |

## Recommended Triggers

This tag is typically fired when:

* A user logs in
* A user creates an account
* User identity becomes available
* User profile data is loaded
* Any authenticated user session event

## Installation

### Option 1: Google Tag Manager Community Template Gallery

Once published, you can install the template directly from the Google Tag Manager Community Template Gallery.

1. Open your GTM container.

2. Navigate to **Templates**.

3. Under **Tag Templates**, click **Search Gallery**.

4. Search for:

   ```
   Common Room Identify Tag
   ```

5. Add the template to your container.

6. Create a new tag using the template.

### Option 2: GitHub Repository

You can also download the latest template release directly from this repository.

1. Download the template file from the repository releases.
2. Open your GTM container.
3. Navigate to **Templates**.
4. Select **Import**.
5. Upload the downloaded template file.
6. Create a new tag using the imported template.

## Permissions

The template requires permission to execute the Common Room Signals identify method.

Depending on your configuration, additional permissions may be required for debug logging.

## Debug Logging

When **Enable Debug Logging** is enabled, the template writes helpful diagnostic messages to the browser console.

This can be useful when:

* Testing implementation
* Verifying field values
* Confirming successful execution
* Troubleshooting Common Room setup issues

It is recommended to disable debug logging in production environments.

## Support

If you encounter issues with the Common Room Signals implementation, consult the official Common Room documentation:

https://www.commonroom.io/docs/signals/website-visitor-tracking/

## More GTM Templates, Tools & Resources

### DumbData

Visit our website:

https://dumbdata.co/

### GTM Custom Templates

Browse additional GTM templates:

https://dumbdata.co/gtm-custom-templates/

### Tools & Templates

Explore free tools and resources:

https://dumbdata.co/tools-and-templates/

### Blog

Read implementation guides, tutorials, and measurement insights:

https://dumbdata.co/blog/

### Free GA4 Audit Tool

https://dumbdata.co/tools-and-templates/free-google-analytics-ga4-audit-tool/

### Free UTM Audit Tool

https://dumbdata.co/tools-and-templates/free-utm-audit-tool/

### Contact Us

Need analytics help, implementation assistance or measurement support?

https://dumbdata.co/contact-us/

## License

Licensed under the Apache License 2.0.

See the LICENSE file for details.
