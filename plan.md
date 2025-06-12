# Project Plan: CloudWeave

**Description:** A simplified web hosting platform built with Ruby on Rails, designed for ease of use and essential features.


## Development Goals

- [ ] Configure tailwindcss-rails by running `rails tailwindcss:install` and customize the `app/assets/stylesheets/application.tailwind.css` file with a basic theme.
- [ ] Implement user authentication using Devise. Set up initial user registration and login forms.
- [ ] Modify the Domain model to belong to a User (add `belongs_to :user` to Domain model).
- [ ] Modify the Domains controller to ensure that only logged-in users can create and manage domains and only see their own domains (Use `before_action :authenticate_user!` and scope queries to `current_user.domains`).
- [ ] Add a form on the user's profile page to allow users to change their password and email address (Devise provides helpers for this).
- [ ] Implement domain status updates (e.g., 'active', 'pending', 'suspended') with appropriate controller actions and views.
- [ ] Add a basic pricing structure and plan options (e.g., 'basic', 'premium') to the Domain model and UI.
- [ ] Implement a simple dashboard view showing the user's domains and account information.
- [ ] Add basic input validations to the Domain model, like validating the domain name format.
- [ ] Customize the scaffold views (index, show, new, edit) with Tailwind CSS for improved aesthetics and usability.
