# PolyForm <%= title %> License

Working Draft

<https://github.com/polyformproject/license-development>

## Acceptance

In order to get free licenses for the software under these terms, you have to agree to all of these terms.

<%# Headline Permission Provisions %>

<% if smallbusiness %>
## Small Business Use

The licenses under these terms allow you to use the software for the benefit of your company only if your company has fewer than 100 total individuals working as employees and independent contractors, and less than 1,000,000 USD (2019) total revenue in the prior tax year.  Adjust this revenue threshold for inflation according to the United States Bureau of Labor Statistics' consumer price index for all urban consumers, U.S. city average, for all items, not seasonally adjusted, with 1982–1984=100 reference base.
<% end %>

<% if internaluse %>
## Internal Business Use

The licenses under these terms allow you to use and change the software only for the internal business operations of you and your company only.
<% end %>

<% if freetrial %>
## Free Trial

The licenses under these terms allow you to use and change the software for yourself or your company for 30 consecutive calendar days, to evaluate whether the software suits a particular application.
<% end %>

<% if noncommercial or strict %>
## Noncommercial Use

The licenses under these terms allow you to use<% if noncommercial %>, change, and share<% end %> the software for noncommercial purposes only.

## Personal Uses

Use for noncommercial purposes includes personal use for research, experiment, and testing for the benefit of public knowledge, personal study, private entertainment, hobby projects, amateur pursuits, or religious observance, without any anticipated commercial application.

## Noncommercial Organizations

Use for noncommercial purposes includes use by any charitable organization, educational institution, public research organization, public safety or health organization, environmental protection organization, or government institution, regardless of the source of funding or obligations resulting from funding.
<% end %>

<% if perimeter or shield %>
## Noncompetitive Use

The licenses under these terms allow you to use, change, and share the software for any purpose other than providing any product that competes with the software<% if shield %> or any product the licensor or any of its affiliates provides using the software<% end %>.

## Competition

<% if shield %>Goods and services compete even when they provide functionality through different kinds of interfaces or for different technical platforms.  Applications can compete with services, libraries with plugins, frameworks with development tools, and so on, even if they're written in different programming languages or for different computer architectures.  Goods and services compete even when provided free of charge.  If you market a product as a practical substitute for the software or another product, it definitely competes.<% end %>
<% if perimeter %>If you use the software to market a product as a substitute for the functionality or value of the software, it competes with the software. A product may compete regardless how it is designed or deployed. For example, a product may compete even if it provides its functionality via any kind of interface (including services, libraries or plug-ins), even if it is ported to a different platform or programming language, and even if it is provided free of charge.<% end %>
<% end %>

<% if shield %>
## New Products

If you are using the software to provide a product that does not compete, but the licensor or any of its affiliates brings your product into competition by providing a new version of the software or another product using the software, you may continue using versions of the software available under these terms beforehand to provide your competing product, but not any later versions.

## Discontinued Products

You may begin using the software to compete with a product or service that the licensor or any of its affiliates has stopped providing, unless the licensor includes a plain-text line beginning with `Licensor Line of Business:` with the software that mentions that line of business.  For example:

> Licensor Line of Business: YoyodyneCMS Content Management System (http://example.com/cms)

## Sales of Business

If the licensor or any of its affiliates sells a line of business developing the software or using the software to provide a product, the buyer can also enforce [Noncompete](#noncompete) for that product.
<% end %>

<%# License Grants %>

## Copyright License

The licensor grants you a copyright license for the software to make copies as needed to run the software<% if change %>, to make changes to the software<% end %><% if distribute %>, and to share copies and changes with others<% end %>.

<% if distribute %>
## Notices

Make sure anyone who gets a copy of any part of the software from you also gets a copy of these terms or the URL for them above, as well as copies of any plain-text lines beginning with `Required Notice:` that the licensor provided with the software.  For example:

> Required Notice: Copyright Yoyodyne, Inc. (http://example.com)
<% end %>

## Patent License

The licensor grants you a patent license for the software that covers patent claims the licensor can license, or becomes able to license, that you would infringe by using the software.

## Fair Use

You may have "fair use" rights for the software under the law. These terms do not limit them.

## No Other Rights

These terms do not allow you to sublicense or transfer any of your licenses to anyone else, or prevent the licensor from granting licenses to anyone else.  These terms do not imply any other licenses.

## Patent Defense

If you make any written claim that the software infringes or contributes to infringement of any patent, your patent license for the software granted under these terms ends immediately. If your company makes such a claim, your patent license ends immediately for work on behalf of your company.

## Violations

The first time you are notified in writing that you have violated any of these terms, or done anything with the software not covered by your licenses, your licenses can nonetheless continue if you come into full compliance with these terms, and take practical steps to correct past violations, within 30 days of receiving notice.  Otherwise, all your licenses end immediately.

## No Liability

***As far as the law allows, the software comes as is, without any warranty or condition, and the licensor will not be liable to you for any damages arising out of these terms or the use or nature of the software, under any kind of legal claim.***

## Definitions

The **licensor** is the individual or entity offering these terms, and the **software** is the software the licensor makes available under these terms.

<% if shield or perimeter %>
A **product** can be a good or service, or a combination of them.
<% end %>

**You** refers to the individual or entity agreeing to these terms.

<% if shield %>
**Your company** is any legal entity, sole proprietorship, or other kind of organization that you work for, plus all its affiliates.

**Affiliates** means the other organizations than an organization has control over, is under the control of, or is under common control with.

**Control** means ownership of substantially all the assets of an entity, or the power to direct its management and policies by vote, contract, or otherwise.  Control can be direct or indirect.
<% else %>
**Your company** is any legal entity, sole proprietorship, or other kind of organization that you work for, plus all organizations that have control over, are under the control of, or are under common control with that organization.  **Control** means ownership of substantially all the assets of an entity, or the power to direct its management and policies by vote, contract, or otherwise.  Control can be direct or indirect.
<% end %>

**Your licenses** are all the licenses granted to you for the software under these terms.

**Use** means anything you do with the software requiring one of your licenses.
