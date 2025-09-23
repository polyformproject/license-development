# PolyForm <%= title %> License

Working Draft

<https://github.com/polyformproject/license-development>

<%# Headline Permission Provisions %>

<% lets_you = 'The licensor gives you permission to' %>

<% if smallbusiness %>
## Small Business Use
<% scope_heading = 'Small Business Use' %>
<% scope_id = 'small-business-use' %>

<%= lets_you %> run this software for the benefit of your company so long as it has fewer than 100 total individuals working as employees and independent contractors and less than 1,000,000 USD (2019) total revenue in the prior tax year.  Adjust this revenue threshold for inflation according to the United States Bureau of Labor Statistics' consumer price index for all urban consumers, U.S. city average, for all items, not seasonally adjusted, with 1982–1984=100 reference base.
<% end %>

<% if internaluse %>
## Internal Business Use
<% scope_heading = 'Internal Business Use' %>
<% scope_id = 'internal-business-use' %>

<%= lets_you %> run and change this software only for the internal business operations of you and your company only.
<% end %>

<% if freetrial %>
## Free Trial
<% scope_heading = 'Free Trial' %>
<% scope_id = 'free-trial' %>

<%= lets_you %> run and change this software for yourself or your company for 30 consecutive calendar days to evaluate whether this software suits a particular application.
<% end %>

<% if noncommercial or strict %>
## Noncommercial Use
<% scope_heading = 'Noncommercial Use' %>
<% scope_id = 'noncommercial-use' %>

<%= lets_you %> run<% if noncommercial %>, change, and share<% end %> this software only for noncommercial purposes.

## Personal Uses

Noncommercial purposes include research, experiment, and testing for the benefit of public knowledge, education, private entertainment, hobby projects, amateur pursuits, and religious observance.

## Noncommercial Organizations

Noncommercial purposes include use on behalf of any charitable organization, educational institution, public research organization, public safety or health organization, environmental protection organization, or government institution.
<% end %>

<% if perimeter or shield %>
## Noncompetitive Use
<% scope_heading = 'Noncompetitive Use' %>
<% scope_id = 'noncompetitive-use' %>

<%= lets_you %> run, change, and share this software for any purpose except providing any product that competes with this software<% if shield %> or any product the licensor or any of its affiliates provides using this software<% end %>.

## Competition

<% if shield %>Goods and services compete even when they provide functionality through different kinds of interfaces or for different technical platforms.  Applications can compete with services, libraries with plugins, frameworks with development tools, and so on, even if they're written in different programming languages or for different computer architectures.  Goods and services compete even when provided free of charge.  If you market a product as a practical substitute for this software or another product, it definitely competes.<% end %>
<% if perimeter %>If you use this software to market a product as a substitute for the functionality or value of this software, it competes with this software.  A product may compete regardless how it is designed or deployed.  For example, a product may compete even if it provides its functionality via any kind of interface (including services, libraries or plug-ins), even if it is ported to a different platform or programming language, and even if it is provided free of charge.<% end %>
<% end %>

<% if shield %>
## New Products

If you are using this software to provide a product that does not compete, but the licensor or any of its affiliates brings your product into competition by providing a new version of this software or another product using this software, you may continue using versions of this software available under this license beforehand to provide your competing product, but not any later versions.

## Discontinued Products

You may begin using this software to compete with a product or service that the licensor or any of its affiliates has stopped providing, unless the licensor includes a plain-text line beginning with `Licensor Line of Business:` with this software that mentions that line of business.  For example:

> Licensor Line of Business: YoyodyneCMS Content Management System (http://example.com/cms)

## Sales of Business

If the licensor or any of its affiliates sells a line of business developing this software or using this software to provide a product, the buyer can also enforce [Noncompete](#noncompete) for that product.
<% end %>

<%# License Grants %>

## Copyrights

The licensor gives you permission under its copyrights in this software to make copies as needed to run this software<% if change %><% if distribute %>, <% else %> and <% end %>to make changes to this software<% end %><% if distribute %>, and to share copies and changes with others<% end %><% if distribute %>, in each case<% end %> under [<%= scope_heading %>](#<%= scope_id %>).

<% if distribute %>
## Notices

Make sure anyone who gets a copy of any part of this software from you also gets a copy of this license or the URL for it above, as well as copies of any plain-text lines beginning with `Required Notice:` that the licensor provided with this software.  For example:

> Required Notice: Copyright Yoyodyne, Inc. (http://example.com)
<% end %>

## Patents

The licensor gives you permission under any patent claims it can license, or becomes able to license, that you would infringe by running<% if change %><% if distribute %>, <% else %> or <% end %>changing<% if distribute %>, or sharing<% end %><% end %> this software<% if distribute %>, in each case<% end %> under [<%= scope_heading %>](#<%= scope_id %>).

## Fair Use

You may have "fair use" rights for this software under the law.  This license doesn't limit those rights.

## No Other Rights

The licensor does not give you permission to sublicense or give your license for this software to anyone else.  The terms of this license aren't meant to imply any other licenses not explicitly mentioned.

## Patent Defense

If you make any claim in writing that this software infringes or contributes to infringement of any patent, your patent permission for this software under this license ends immediately.  If your company makes a claim, the patent part of your license ends immediately for work on behalf of your company.

## Violations

The first time you get notified in writing that you've violated any term of this license, or gone beyond the permissions given under it, your license can nonetheless continue if you come into full compliance with these terms, and take practical steps to correct past violations, within 30 days of receiving notice.  Otherwise, both the copyright and patent parts of this your license end immediately.

## No Liability

***As far as the law allows, this software comes as is, without any warranty or condition, and the licensor will not be liable to you for any damages arising out of this license or the use or nature of this software, under any kind of legal claim.***

## Definitions

The **licensor** is the individual or entity offering this license.

**You** refers to the individual or entity agreeing to these terms.

<% if shield or perimeter %>
A **product** can be a good or service, or a combination of them.
<% end %>

<% if shield %>
**Your company** is any legal entity, sole proprietorship, or other kind of organization that you work for, plus all its affiliates.

**Affiliates** means the other organizations than an organization has control over, is under the control of, or is under common control with.

**Control** means ownership of substantially all the assets of an entity, or the power to direct its management and policies by vote, contract, or otherwise.  Control can be direct or indirect.
<% else %>
**Your company** is any legal entity, sole proprietorship, or other kind of organization that you work for, plus all organizations that have control over, are under the control of, or are under common control with that organization.

**Control** means ownership of substantially all the assets of an entity, or the power to direct its management and policies by vote, contract, or otherwise.  Control can be direct or indirect.
<% end %>

**Use** means anything you do with this software requiring a license under copyright or patent law.
