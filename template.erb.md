# PolyForm <%= title %> License

Working Draft

<https://github.com/polyformproject/license-development>

<%# Headline Permission Provisions %>

<% def business (headcount, revenue) "You may run this software for the benefit of your company so long as it has fewer than #{headcount} total individuals working as employees and independent contractors and less than #{revenue} USD (2019) total revenue in the prior tax year.  Adjust this revenue threshold for inflation according to the United States Bureau of Labor Statistics' consumer price index for all urban consumers, U.S. city average, for all items, not seasonally adjusted, with 1982–1984=100 reference base." end %>

<% if smallbusiness %>
## Small Business Use
<% scope_heading = 'Small Business Use' %>
<% scope_id = 'small-business-use' %>
<%= business('50', '10,000,000') %>
<% end %>

<% if microbusiness %>
## Micro Business Use
<% scope_heading = 'Micro Business Use' %>
<% scope_id = 'micro-business-use' %>
<% scope_id = 'small-business-use' %>
<%= business('10', '2,000,000') %>
<% end %>

<% if internaluse %>
## Internal Business Use
<% scope_heading = 'Internal Business Use' %>
<% scope_id = 'internal-business-use' %>

You may run and make changes to this software only for the internal business operations of you and your company.
<% end %>

<% if freetrial %>
## Free Trial
<% scope_heading = 'Free Trial' %>
<% scope_id = 'free-trial' %>

You may run and make changes to this software for yourself or your company for 30 calendar days in a row, only to find out whether this software will work for a particular need or project.  You may try this software for multiple different needs and projects for 30 days each.
<% end %>

<% personal_uses = 'Noncommercial purposes include research, experiment, and testing for the benefit of public knowledge, education, private entertainment, hobby projects, amateur pursuits, and religious observance.' %>

<% if noncommercial or strict %>
## Noncommercial Use
<% scope_heading = 'Noncommercial Use' %>
<% scope_id = 'noncommercial-use' %>

You may run<% if noncommercial %>, make changes to, and share<% end %> this software only for noncommercial purposes.

## Personal Uses

<%= personal_uses %>

## Noncommercial Organizations

Noncommercial purposes include work on behalf of any charitable organization, educational institution, public research organization, public safety or health organization, environmental protection organization, or government institution.
<% end %>

<% if personaluse %>
## Personal Use
<% scope_heading = 'Personal Use' %>
<% scope_id = 'personal-use' %>

You may run, make changes to, and share this software only for personal noncommercial purposes unaffiliated with any organization.  <%= personal_uses %>
<% end %>

<% if perimeter or shield %>
## Noncompetitive Use
<% scope_heading = 'Noncompetitive Use' %>
<% scope_id = 'noncompetitive-use' %>

You may run, make changes to, and share this software for any purpose except providing any product that competes with this software<% if shield %> or any product the licensor or any of its affiliates provides using this software<% end %>.

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

<% if shield or perimeter %>
## Products

Throughout this license, _product_ is used to mean a good, service, or combination of them.
<% end %>

<%# License Grants %>

## Copyrights

The licensor gives you permission under its copyrights in this software to run<% if change %><% if distribute %>, <% else %> and <% end %>make changes to<% end %><% if distribute %>, and share copies of and changes to<% end %> this software<% if change %>, but only<% end %> as allowed by [<%= scope_heading %>](#<%= scope_id %>).

<% if distribute %>
## Notices

Make sure anyone who gets a copy of any part of this software from you also gets a copy of this license or the URL for it above, as well as copies of any plain-text lines beginning with `Required Notice:` that the licensor provided with this software.  For example:

> Required Notice: Copyright Yoyodyne, Inc. (http://example.com)
<% end %>

## Patents

The licensor gives you permission under any patent claims it can license, or becomes able to license, that you would infringe by running<% if change %><% if distribute %>, <% else %> or <% end %>changing<% if distribute %>, or sharing<% end %><% end %> this software<% if change %>, but only<% end %> as allowed by [<%= scope_heading %>](#<%= scope_id %>).

## Fair Use

This license doesn't limit "fair use" under copyright law.

## No Other Rights

You may not sublicense or transfer your license for the software to anyone else.  The terms of this license don't imply any other licenses.

## Patent Defense

If you claim in writing that this software infringes or contributes to infringement of any patent, your patent permission under this license ends immediately.  If your company claims in writing that this software infringes or contributes to infringement of any patent, your patent permission ends immediately for work on behalf of your company.

## Violations

The first time the licensor warns you in writing that you've violated any term of this license, or used this software in a way this license doesn't allow, your license can nonetheless continue if you come into full compliance with this license, and take practical steps to correct past violations, within 30 days.  Otherwise, your copyright and patent permission under this license ends immediately.

## No Liability

***As far as the law allows, this software comes as is, without any warranty or condition, and the licensor will not be liable to you for any legal damages arising out of this license or the use or nature of this software, under any kind of legal claim.***

## You and Your Company

Throughout this license, _you_ refers to the individual or legal entity agreeing to these terms, and _your company_ refers to any legal entity, sole proprietorship, or other kind of organization that you work for, plus all of its affiliates, plus all organizations that have control over, are under the control of, or are under common control with that organization.  _Control_ means ownership of substantially all the assets of an organization, or the power to direct its management and policies by vote, contract, or otherwise.  Control can be direct or indirect.
