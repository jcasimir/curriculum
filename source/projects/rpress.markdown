---
layout: page
title: RPress
---

In this project you'll use Ruby on Rails to build a content management system.

<div class="note">
<p>Consider the requirements fluid until 11:59PM, Monday, April 30th.</p>
</div>

### Learning Goals

* Practices techniques for scalable application architecture including caching, pre-rendering, and database optimization.
* Continue using TDD to drive all layers of Rails development
* Continue to improve User Interface concepts and skills

### Understandings

Please consider the requirements below non-exhaustive guidelines for building a content management system. If you know something should be done but it isn't listed below, do it.

### Restrictions

Project implementation may *not* use:

* RadiantCMS, RefineryCMS, or any other pre-fab CMS system
* Jekyll or derivitives

### Base Expectations

You are to build a content management system which can be used by administrators to create content and public users to consume content.

#### Public Visitor

As a public visitor I can:

* View content on the site
* Access the login page

#### Authenticated Author

As an authenticated author, I can:

* Manipulate Content (assuming I'm authorized)
  * Create/Edit/Delete pages
  * Create/Edit/Delete snippets 
  * Create/Edit/Delete redirects
* My Account
  * Login
  * Request a password reset and receive a login link via email
  * Change my password
  * View my login history (timestamps, IP address)

#### Authenticated Administrator

As an authenticated Administrator, I can:

* Do everything an Author can do
* Accounts
  * Create new accounts 
  * Change the password of a specified account
  * Generate a random-ish password which is emailed to the account owner
  * Deactivate an account
* Permissions
  * Create permissions groups (ex: "Blog Authors")
  * Assign and remove accounts from permissions groups
  * Connect permissions groups with pages (see later section)

### Permissions / Authorization

( Here's how the permissions model is going to work )

( Groups are assigned to a page and it trickles down through the hierarchy )

### Creating Content

#### Pages

( Pages have a title, body, slug )

#### Layouts

( Layouts wrap content )

( Layouts can be nested inside other layouts )

#### Snippets

( Snippets )

#### Redirects

( Redirects match specific paths )

( Extension: redirects match flexible paths with wildcards, etc)

#### Assets

( Assets can be uploaded )

### Data Validity

Any attempt to create/modify a record with invalid attributes should return the user to the input form with a validation error indicating the problem along with suggestions how to fix it.

#### Page

* must have a name unique to that level of the page hierarchy
* must be attached to a layout

#### Snippet

* must have a name unique to that collection

#### Layout

* must have a unique name

#### Redirects

* must have an order of precidence
* must have a destination

### Example Data

### Extensions

#### 1

#### 2

#### 3

#### 4

### Evaluation Criteria

This project will be peer assessed using automated tests and the rubric below. Automated tests will be available by 8AM, Tuesday, April 10th.

1. Correctness
  * 3: All provided stories pass without an error or crash
  * 2: One story failed
  * 1: Two or three stories failed
  * 0: More than three stories failed
2. Testing
  * 3: Testing suite covers >95% of application code
  * 2: Testing suite covers 85-94% of application code
  * 1: Testing suite covers 70-84% of application code
  * 0: Testing suite covers <70% of application code
3. Code Style
  * 3: Source code generates no complaints from Cane or Reek.
  * 2: Source code generates warnings about whitespace/comments, but no violations of line-length or method statement count
  * 1: Source code generates six or fewer warnings about line-length or method statement count
  * 0: Source code generates more than six warnings about line-length or method statement count
4. Live Hungry
  * 4: Program fulfills all Base Expectations and four Extensions
  * 3: Program fulfills all Base Expectations and two Extensions
  * 2: Program fulfills all Base Expectations
  * 1: Program is missing 1-3 Base Expectations
  * 0: Program fulfills many Base Expectations, but more than three features are missing.
5. User Interface & Design
  * 3: WOW! This site is beautiful, functional, and clear.
  * 2: Very good design and UI that shows work far beyond dropping in a library or Bootstrap.
  * 1: Some basic design work, but doesn't show much effort beyond "ready to go" components/frameworks/etc
  * 0: The lack of design makes the site difficult / confusing to use
6. Surprise & Delight
  * 2: A great idea that's well executed and enhances the shopping experience.
  * 1: An extra feature that makes things a little nicer, but doesn't blow your mind.
  * 0: No surprise. Sad face :(

### Evaluation Protocol
