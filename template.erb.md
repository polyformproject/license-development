# PolyForm <%= title %> License

Working Draft

<https://github.com/polyformproject/license-development>

<%# Headline Permission Provisions %>

<% def business (headcount, revenue, assets) "You may run this software for the benefit of your company so long as it has fewer than #{headcount} total individuals working as employees and independent contractors, less than #{revenue} USD (2019) total gross revenue in the last tax year, and less than #{assets} USD (2019) total assets as of the end of the last tax year.

<!-- Note: The phrase 'your company' is defined to include afiliates in the 'You and Your Company' section below. -->

Adjust these dollar thresholds for inflation according to the United States Bureau of Labor Statistics' consumer price index for all urban consumers, U.S. city average, for all items, not seasonally adjusted, with 1982–1984=100 reference base.

If your company is a new company that did not pay tax for the last tax year, you may run this software for the benefit of your company during the current tax year until it exceeds the headcount, revenue, and assets figures above." end %>

<% if smallbusiness %>
## Small Business Use
<% permission_scope = 'for small business' %>
<%= business('50', '10,000,000', '10,000,000') %>
<% end %>

<% if microbusiness %>
## Micro Business Use
<% permission_scope = 'for micro business' %>
<%= business('10', '2,000,000', '2,000,000') %>
<% end %>

<% if internaluse %>
## Internal Business Use
<% permission_scope = 'for internal business' %>

You may run and make changes to this software only for the internal business operations of you and your company.
<% end %>

<% if freetrial %>
## Free Trial
<% permission_scope = 'for free trials' %>

You may run and make changes to this software for yourself or your company for 30 calendar days in a row, only to find out whether this software will work for a particular need or project.  You may try this software for multiple different needs and projects for 30 days each.
<% end %>

<% personal_uses = 'Research, experiment, and testing for the benefit of public knowledge, education, private entertainment, hobby projects, amateur pursuits, and religious observance are all noncommercial uses.' %>

<% if noncommercial or strict %>
## Noncommercial Use
<% permission_scope = 'for noncommercial uses' %>

This license gives you free permission for this software, but only for noncommercial uses. The next two sections give examples of noncommercial uses, but do not rule out others.

## Personal Uses

<%= personal_uses %>

## Noncommercial Organizations

Work on behalf of any charitable organization, educational institution, public research organization, public safety or health organization, environmental protection organization, or government institution is a noncommercial use.
<% end %>

<% if personaluse %>
## Personal Use
<% permission_scope = 'for personal noncommercial uses' %>

You may run, make changes to, and share this software only for personal noncommercial uses unaffiliated with any organization.  <%= personal_uses %>
<% end %>

<% if perimeter or shield %>
## Noncompetitive Use
<% permission_scope = 'for noncompetitive purposes' %>

You may run, make changes to, and share this software for any purpose except providing any product that competes with this software<% if shield %> or any product the licensor or any of its affiliates provides using this software<% end %>.

## Competition

<% if shield %>Goods and services compete even when they provide functionality through different kinds of interfaces or for different technical platforms.  Applications can compete with services, libraries with plugins, frameworks with development tools, and so on, even if they're written in different programming languages or for different computer architectures.  Goods and services compete even when provided free of charge.  If you market a product as a practical substitute for this software or another product, it definitely competes.<% end %>
<% if perimeter %>If you use this software to market a product as a substitute for the functionality or value of this software, it competes with this software.  A product may compete regardless how it is designed or deployed.  For example, a product may compete even if it provides its functionality via any kind of interface (including services, libraries or plug-ins), even if it is ported to a different platform or programming language, and even if it is provided free of charge.<% end %>
<% end %>

<% if shield %>
## New Products

If you are using this software to provide a product that does not compete, but the licensor or any of its affiliates brings your product into competition by providing a new version of this software or another product using this software, you may continue using versions of this software available under this license beforehand to provide your competing product, but not any later versions.

## Discontinued Products

You may begin using this software to compete with a product or service that the licensor or any of its affiliates has stopped providing, unless the licensor includes a plain-text line beginning with `Licensor Line of Business:` with this software that mentions that line of business.

## Sales of Business

If the licensor or any of its affiliates sells a line of business developing this software or using this software to provide a product, the buyer can also enforce [Noncompete](#noncompete) for that product.

<% end %>

<% if shield or perimeter %>
## Products

Throughout this license, _product_ is used to mean a good, service, or combination of them.
<% end %>

<%# License Grants %>

## Copyrights

The licensor gives you permission under its copyrights in this software to run, make copies of<% if change %><% if distribute %>, <% else %> and <% end %>make changes to<% end %><% if distribute %>, and share copies of and changes to<% end %> this software<% if change %>, but only<% end %> <%= permission_scope %>.

## Patents

The licensor gives you permission under any patent claims it can license, or becomes able to license, that you would infringe by running, copying<% if change %><% if distribute %>, <% else %> or <% end %>changing<% if distribute %>, or sharing<% end %><% end %> this software<% if change %>, but only<% end %> <%= permission_scope %>.

<% if distribute %>
## Notices

Make sure anyone who gets a copy of this software from you also gets a copy of this license or the URL for it above, as well as copies of any plain-text lines beginning with `Required Notice:` that the licensor provided with this software.
<% end %>

## Fair Use

This license does not limit "fair use" under copyright law.

## No Other Rights

You may not sublicense or transfer your permission under this license to anyone else. The terms of this license do not imply any other permission.

## Patent Defense

If you claim in writing that this software infringes or contributes to infringement of any patent, your patent permission under this license ends immediately. If your company claims in writing that this software infringes or contributes to infringement of any patent, your patent permission under tihs license ends immediately for work on behalf of your company.

## Violations

The first time the licensor warns you in writing that you have violated any term of this license or done anything with the software not permitted by this license, your copyright and patent permission under this license can nonetheless continue if you come into full compliance with this license, and take practical steps to correct past violations, within 30 days. Otherwise, your copyright and patent permission under this license ends immediately.

## No Liability

***As far as the law allows, this software comes as is, without any warranty or condition. As far as the law allows the licensor will not be liable to you for any legal damages related to this license or this software, under any kind of legal claim.***

## You and Your Company

Throughout this license, _you_ refers to the individual or legal entity agreeing to these terms, and _your company_ refers to any legal entity, sole proprietorship, or other kind of organization that you work for, plus all organizations that have control over, are under the control of, or are under common control with that organization. _Control_ means ownership of substantially all the assets of an organization or the power to direct its management and policies by vote, contract, or otherwise.
