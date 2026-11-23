# TravelEase – Travel Planning Website

TravelEase is a travel-focused web project designed to bring useful trip-discovery and planning features together in one place. The website showcases popular destinations across India and includes separate pages for hotel/resort information, travel buddy discovery, account forms, map-based destination exploration, and language translation.

I created this project to practise building a multi-page frontend experience and explore how different web technologies and third-party services can support a travel website.

## Project Features

- **Destination discovery:** A TravelEase homepage showcasing tourist destinations across India, with destination highlights and travel inspiration.
- **Hotel and resort page:** A dedicated hotel/resort interface with accommodation highlights, gallery, reservation section, contact area, FAQs, and reviews.
- **Travel Buddy Finder:** A separate experience where users can provide profile details and personality information to support travel-buddy discovery.
- **Account and profile UI:** Signup/account-related pages and profile details.
- **Map-based exploration:** A page with embedded Google Maps locations to help visitors explore destinations and surrounding areas.
- **Language translation:** Google Translate integration to offer page translation.
- **Interactive UI:** JavaScript-driven navigation, sliders, testimonials, and other page interactions.

> Note: These are features represented in the repository code. External integrations such as Firebase and Google Translate require working configuration and should be tested in the deployment environment. This repository should be treated as a learning/demo project rather than a production booking service.

## Technologies Used

- **HTML5** – structure and content across the website pages.
- **CSS3** – custom page styling and layouts.
- **JavaScript** – frontend interactions and dynamic UI behaviour.
- **Firebase (Authentication / Realtime Database SDK)** – used by the Travel Buddy Finder code for account-related and profile data flows.
- **Google Maps embeds** – destination and locality exploration.
- **Google Translate** – page translation widget.
- **Font Awesome** – icons.
- **Swiper.js** – sliders for hotel/resort content.
- **External image assets** – destination, hotel, and profile imagery.

## Project Structure

```text
TravelEase/
├── travel_ease.html       # Main TravelEase destination website
├── hotel-booking.html     # Hotel and resort information page
├── buddy_finder.html      # Travel Buddy Finder page
├── map1.html              # Destination maps and locality exploration
├── login_form.html        # Signup/login-related interface
├── form.html              # Account-created confirmation page
├── g-translator.html      # Google Translate experiment
├── javascript.html        # JavaScript practice page
├── css/
│   ├── travel_ease.css
│   ├── hotel-booking.css
│   ├── buddy_finder.css
│   ├── map.css
│   ├── form.css
│   └── style.css
├── js/
│   ├── script.js
│   ├── hotel.js
│   └── buddy_finder.js
└── images/
    └── Destination, hotel, gallery, and profile images
```

## Run Locally

The project is made primarily of static HTML, CSS, and JavaScript files.

1. Clone the repository:

   ```bash
   git clone https://github.com/Nancyrana1/TravelEase.git
   ```

2. Open the project directory:

   ```bash
   cd TravelEase
   ```

3. Start a local web server from the project folder. For example, use the **Live Server** extension in Visual Studio Code.

4. Open `travel_ease.html` in the browser through the local server.

Other pages can be opened directly through their filenames, such as `hotel-booking.html`, `buddy_finder.html`, and `map1.html`.

## Firebase Setup – Travel Buddy Finder

The Travel Buddy Finder scripts include Firebase Authentication and Realtime Database SDK usage.

To run this part of the project with your own Firebase project:

1. Create a Firebase project.
2. Register a web app and copy its configuration.
3. Configure the Authentication provider(s) used by your implementation.
4. Set up the Realtime Database and appropriate security rules.
5. Update the Firebase configuration in `js/buddy_finder.js` with your own project settings.
6. Test signup, profile saving, profile retrieval, and the personality information flow.

**Security:** Do not commit private credentials or unrestricted service credentials to a public repository. Firebase web API keys are generally identifiers rather than secret passwords, but access must be protected by correctly configured Firebase Authentication, database security rules, and any applicable API restrictions. Review the currently committed configuration and rotate/restrict it if necessary.

## Notes and Limitations

- The repository contains multiple standalone HTML pages; use `travel_ease.html` as the main TravelEase entry point.
- The map page uses Google Maps embed URLs, so it requires an internet connection.
- Google Translate and other CDN-hosted libraries also require internet access.
- Firebase-backed pages will not work as intended until the Firebase project configuration and security rules are valid.
- Booking and reservation interfaces should not be interpreted as a connected, live hotel inventory or payment system unless a backend integration is added and verified.

## What I Learned

Working on TravelEase gave me the opportunity to practise:

- Building and organizing a multi-page website.
- Creating navigation between related pages and user flows.
- Designing destination and hotel/resort layouts with HTML and CSS.
- Using JavaScript to add interactive elements.
- Integrating external services such as Firebase, Google Maps, and Google Translate.
- Working with image galleries, sliders, and responsive layout techniques.
- Organizing a project into separate HTML, CSS, JavaScript, and image folders.
- Understanding that third-party integrations need configuration, security rules, and testing.

## Future Improvements

- Consolidate repeated styles and scripts and improve overall code organization.
- Make all pages consistently responsive and accessible.
- Complete and test the login, signup, and travel-buddy matching flows.
- Add proper validation and secure database access rules.
- Connect hotel reservation forms to a backend and real availability data.
- Replace static destination/map content with searchable, verified location data.
- Improve error handling, loading states, and user feedback.
- Add screenshots and a deployed demo link to this README.

## Disclaimer

TravelEase is an independent educational project. It is not affiliated with or endorsed by any travel agency, hotel chain, mapping provider, or other service mentioned. Destination descriptions and booking-related interfaces are provided for demonstration and learning purposes only.

## Author

Created by [Nancyrana1](https://github.com/Nancyrana1) as a web development project while exploring frontend development and third-party web integrations.

Feedback and suggestions are welcome!
