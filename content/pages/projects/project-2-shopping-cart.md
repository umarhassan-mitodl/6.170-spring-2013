---
content_type: page
description: This section provides a project overview, the list of deliverables, and
  hints for a project to build a basic shopping card application.
learning_resource_types:
- Projects
ocw_type: CourseSection
parent_title: Projects
parent_type: CourseSection
parent_uid: 1b52d2eb-781f-59fc-2005-cfdb8156e288
title: 'Project 2: Shopping Cart'
uid: 20735433-db81-6010-17a0-c8daa1a923e7
---

Overview
--------

Online stores ({{% resource_link "d38cd7fc-29e9-4a49-bed1-142bcbd1d610" "Amazon" %}}, {{% resource_link "b90b0e1f-324f-41cd-aeaa-98ebc4d8d9a2" "Newegg" %}}, {{% resource_link "b4edb9e2-af63-43e5-86cf-08340deed51d" "Zappos" %}}, {{% resource_link "a31fd48a-a8c9-4c6d-a172-89dc397bd572" "Half.com" %}}) offer the notion of a shopping cart. Just as MP3 players often have a "rewind" button even though the physical notion of rewinding no longer exists, shoppers have come to expect an online cart to have the same features as a physical cart: temporarily holding items until purchase, removals and additions, and so on. Website visitors can usually place items in a cart before logging in or identifying themselves, and may be able to retain a cart's contents across sessions. Large retailers typically implement their own shopping cart applications, but smaller ones often use third-party services, such as {{% resource_link "4ec8e191-2eb4-4440-9155-27cfd786df83" "Opencart" %}}, {{% resource_link "5b5e0779-8346-468b-b6bf-128b454b26e2" "Shopify" %}}, {{% resource_link "e036256c-89bd-4d10-9283-4d5133d17f15" "PayPal" %}}, and {{% resource_link "20bd59a1-f009-4a6e-9574-c6cdac237c48" "Stripe" %}}.

In this project, you will implement a basic shopping cart application with two user interfaces: one for a shopper (for purchasing items), and one for a shopkeeper (for editing the catalog of items and for reviewing orders).

Deliverables
------------

### Phase 1: Design of Minimum Viable Product

**Minimal requirements.** In the first two phases, you'll design and implement a basic shopping website with these minimal requirements:

*   User interface for shopper, including the ability to add and remove items from cart, view cart, and place order (but no real payment needed)
*   User interface for shopkeeper, including the ability to create and modify catalog of items and prices, and to view recent orders from customers

In the first phase, you will construct only a paper design.

**Checklist items.** Of the items specified on the project checklist, you should include in this phase:

*   Design: all parts, except for Design/Evaluation, and notes on code design (under Design/Challenges).

### Phase 2: Implemention of Minimum Viable Product

In this phase, you will build an implementation of the design you did in Phase 1.

**Checklist items.** Of the items specified on the project checklist, you should include in this phase:

*   Programming: all sections, except unit tests
*   Design: a revised version that includes a fuller Design/Challenges section

### Phase 3: Your Own Shopping Cart

**Minimal requirements.** In this phase, you will complete your project by polishing it and adding one feature from the list below:

*   Saved items: Items or entire carts can be saved for purchase later.
*   Shopping lists: Lists can be shared between shoppers (_e.g._, for gifts).
*   Internationalization: System allows multiple languages.
*   Web service: Code is refactored so it can be used as a service rather than a custom site.

**Checklist items.** Of the items specified on the project checklist, you should include in this phase:

*   Programming: all parts, excluding unit tests
*   Design: all parts (except for design critique), expanded for the new functionality

### Phase 4: Critique

**Minimal requirements**. This phase involves no new design or implementation work. Instead, you will write two short critiques: one of your own work, and one of your peer's work. In addition to checking the critiques into your own repository, you should post your peer critique as one or more issues in your peer's repository.

**Checklist items.** You should include in this phase:

*   Design/Evaluation/Critique for each of the two projects
*   Design/Evaluation/Reflection for your own project

Hints
-----

**Strategy.** In this project, you are asked to do a design on paper before you do any implementation at all. This is intended to give you some experience focusing on high-level design issues before you jump into coding details. If you do it right, you should be able to save yourself time overall (so that the whole project takes less time than it would if you just hacked the code). To get this advantage, you will need to use the design analysis as an opportunity to (a) focus on exactly what you plan to do and why, eliminate any extraneous complexities, make suitable generalizations, and figue out how to exploit the features of Rails (_e.g._, RESTful resources); (b) prepare an object model that can be transformed very directly into code; and (c) anticipate some of the tricky issues that might derail the implementation. Your design document should be clear and complete enough that someone else could implement your design without requiring more information from you.

**Security.** At this point, we have not yet covered security threats and mitigations, so we do not expect your analysis or your code to reflect an understanding of technical attacks such as cross site request forgery. We do, however, expect you to be able to address the problem-specific security concerns and implement appropriate mechanisms (for example, using passwords to protect accounts, and using access control to prevent unauthorized access to other people's records).

**Double submission.** Early shopping carts suffered from the problem that pressing the checkout button twice could cause the order to be made twice. Make sure you handle this and related cases properly.