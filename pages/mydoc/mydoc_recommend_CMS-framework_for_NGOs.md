---
title: Recommend CMS/Framework for NGOs
tags: [article, support, security-assessment]
keywords: web security, websites, CMS, framework, static site generators
summary: Best practices for building, creating, and rebuilding a secure website
sidebar: mydoc_sidebar
permalink: mydoc_recommend_CMS-framework_for_NGOs.html
folder: mydoc
---


# Recommend CMS/Framework for NGOs
## Best practices for building, creating, and rebuilding a secure website
### Problem

- The client is uncertain about the best web technology to use to build their website.
- The owner of the website finds it difficult to maintain it for several reasons: lack of technical skills, budget limitations, a wish to rebuild it.
- The website contains submission forms, donation forms, or other forms that permit storing or compromising visitors' data information.
- In certain cases, if the website is compromised, the whole IT architecture of the organization may be compromised.


### Solution

The choice of what to recommend for a web building technology that ensures greater security depends on many factors. Incident handlers should try to assess the needs of the organization. So, even if the client is asking specifically for a Framework or CMS recommendation, we should try to propose changes and improvements wherever the organization needs them.

The following questions might help us have a better understanding of the client’s needs: 

- Is it a static or dynamic website? 
- What are the contents and features of the website? What is the intention of the website?
- Does the client have a technical person available with the necessary expertise? Will this person maintain the website or not?
- If the client wants to rebuild their website, what is the current architecture? CMS, development language, DB server (SQL database, flat-file DB type) technology, server type (LAMP, IIS), one-person publisher, etc.? Remote installation, or on local machine only?

We need to take into consideration all security concerns when providing the client with recommendations. Providing more than one proposition to the client (top 3), with pros and cons, allows the client to decide the solution that best fits their need.

We should only recommend FOSS solutions, and we shouldn't recommend online site makers because the hoster owns the source code of the website.

We need to explain to the client that a CMS needs a webmaster to handle upgrades and other security issues, and they cannot install a CMS and just leave it as it is forever.

Also, every web technology has its vulnerabilities and flaws, especially if it's not well implemented and maintained (system up to date, security patches, etc.).

The security of the website doesn't only depend on the best chosen CMS/Framework - every environment or technology should be installed, configured and secured appropriately; the same applies to the web server, DB server, host server, production environment, source code of the website, plugins, HTTPS configuration, DDOS protection, etc.

#### CMS or Framework - what is the best?

Generally, clients ask for a tool to develop an organization’s official website or a small simple website with mostly text content. In these scenarios, we would usually propose a CMS. 

Sometimes, the client could have a technical person with some framework skills; all frameworks have the same design, so we could propose a Framework instead of a CMS.


#### CMSs: Drupal, Joumla, or Wordpress?

- **Wordpress** could be the best choice for a simple blog or brochure-type site (while very friendly for non-developers, it’s a flexible platform also capable of very complex sites).
- **Drupal** is best suited for a complex, highly customized site requiring scalability and complex content organization. Operating it requires a certain degree expertise and experience. 
- **Joomla** can be recommended as something in between that has an easier learning curve.


#### Static website technologies

It may be good to investigate and add one or more static website options, given their security benefits:

- [**Nikola**](https://getnikola.com/)
- [**Jekyll**](http://jekyllrb.com, https://en.wikipedia.org/wiki/Jekyll_(software))
- [**Octopress** (built on top of Jekyll)](https://github.com/octopress/octopress)
- [**Pelican**](http://blog.getpelican.com/) - Pelican is a static site generator, written in Python, that requires no database or server-side logic.
- [**MkFramework**](http://mkframework.com/) - For mini forums building, a very interesting Framework project (website in French)
- [**Hugo**](https://gohugo.io/) - A fast and flexible static site generator built in Go.
- [**Mezzanine**](http://mezzanine.jupo.org/)


### Comments

[List of content management systems](https://en.wikipedia.org/wiki/List_of_content_management_systems)

[This website](https://www.opensourcecms.com) has demo versions of over 70 open source LAMP-based CMSs, including Drupal, Mambo, and Joomla, eZ publish, Lenya, and phpBB.

[This website](http://www.cmsmatrix.org/matrix/cms-matrix) lets you make the comparison between two or more CMSs from a features/functionalities perspective.

[This is a good reference for a Secure Configuration Guide](https://www.owasp.org/index.php/Secure_Configuration_Guide).

