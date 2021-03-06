---
layout: page
weight: 0
title: CNAME
seo:
  title: CNAME
  override: true
  description: The CNAME record creates an alias for subdomain.yourdomain.com and points it to another domain
navigation:
  show: false
---

The CNAME record creates an alias for subdomain.yourdomain.com and points to sendgrid.net. The CNAME is needed for our click and open tracking features in order for those statistics to be routed back to your SendGrid account. This will also be what your messages are signed by, so your recipients will be able see what you have chosen for your CNAME.

What it should look like:

{% codeblock %}
subdomain.yourdomain.com.  |  CNAME  |  sendgrid.net.
{% endcodeblock %}

If your account has a dedicated IP and you are looking to [whitelabel]({{root_url}}/User_Guide/Setting_Up_Your_Server/Whitelabeling/index.html) your IP, you will need to add some records to your DNS host. In this group of records you will have 1 CNAME record.

If you are having trouble validating your CNAME record, please see our [Classroom]({{root_url}}/Classroom/Troubleshooting/Authentication/i_have_created_dns_records_but_the_whitelabel_wizard_is_not_validating_them.html).
