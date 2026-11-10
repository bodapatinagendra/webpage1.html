🚌 PALLEVELUGU LIVE
Know Your Bus, Plan Your Journey
PALLEVELUGU LIVE is a frontend web application prototype for passenger information and journey planning for APSRTC and TGSRTC services in Andhra Pradesh and Telangana.
The project brings together bus route search, district-wise stop selection, route mapping, timetable display, passenger profile options, logistics information, food information, and emergency/help options in one webpage.
> **Project status:** This repository contains a frontend demonstration. It does not currently connect to an official APSRTC/TGSRTC live GPS, timetable, reservation, or seat-inventory system. Bus schedules and seat availability shown in the demo are sample data.
---
✨ Features in This Project
1. Bus route search
Select a transport state: Andhra Pradesh or Telangana.
Select a district from the available district list.
Choose pickup and drop-off stops from district-specific suggestions.
Search using a journey date and preferred time.
Validate that both stops belong to the selected district and are different.
2. District and bus-stop information
Includes district lists for Andhra Pradesh and Telangana.
Provides searchable city and bus-stop suggestions.
Uses stored coordinates for selected stops.
Some stop entries are generated from major city/town demo data.
Note: The stop list is a planning/demo dataset, not an official or exhaustive RTC stop database.
3. Route map and navigation
Interactive map using Leaflet.js.
Map tiles from OpenStreetMap.
Pickup and drop-off markers.
Road-route request using the OSRM routing service.
Displays estimated road distance and approximate bus travel time.
Shows a straight-line fallback if road routing is unavailable.
Reset map option.
Links to open the selected route in Google Maps or Apple Maps.
Note: The travel-time estimate uses an assumed average speed of 38 km/h. It is not a live bus ETA or GPS position.
4. Bus timetable demonstration
Displays sample bus services after a route search.
Shows bus number/name, departure, arrival, and status.
Displays an available-bus count.
Includes sample Pallevelugu and RTC service entries.
Note: Timetable rows are hard-coded demo schedules, not live RTC timetable results.
5. Seat availability demonstration
Displays a 24-seat sample bus layout.
Shows available, selected, and booked seat states.
Allows passengers to select and deselect seats.
Limits selection to a maximum of four seats.
Accepts passenger name and mobile number.
Updates the seat counts after a demo booking.
Note: Seat status is held in browser JavaScript memory. It is not connected to an RTC reservation system or shared database, and bookings are not permanently stored.
6. Passenger profile
Profile dropdown with passenger information.
Edit-profile form for name, age, sex, mobile number, email, and profile image URL.
Login/register modal interface.
Referral form interface.
Note: The profile and login screens are frontend demonstrations. There is no authentication or permanent profile storage in this HTML file.
7. Enquiry and support
General bus enquiry/contact form.
Help and support modal with basic route-search instructions.
Complaint/grievance form with a demo reference number.
Emergency assistance buttons for calling the configured helpline numbers.
8. Logistics
Cargo and parcel logistics interface.
Tracking/AWB number and mobile-number fields.
Note: The logistics form does not query an actual parcel tracking service.
9. Food information
Food section accessible from the navigation menu.
Displays the selected district and journey route in its interface.
10. User interface
Dark and light theme options.
Responsive layout for smaller screens.
Recent route searches stored in browser `localStorage`.
Clear recent-search history option.
RTC updates ticker linking to the APSRTC website.
Navigation menu, profile dropdown, modal dialogs, and animated UI elements.
---
🧰 Technologies and Services
Technology / Service	Use
HTML5	Page structure and forms
CSS3	Layout, themes, responsive styling, and animations
JavaScript	Search logic, validation, menus, modals, and interactions
Leaflet.js	Interactive map display
OpenStreetMap	Map tile data
OSRM	Road-route geometry and road-distance estimate
Browser Local Storage	Save recent route searches
Google Maps	External route navigation
Apple Maps	External route navigation
---
📁 Project Structure
The uploaded project is currently provided as a single HTML page:
```text
PALLEVELUGU-LIVE/
│
├── webpage1.html
├── README.md
└── rtclogo.png          # Optional local RTC logo used by the page
```
Keep `rtclogo.png` in the same folder as the HTML file if you want the local logo to appear. The page also loads Leaflet and map tiles from external services, so an internet connection is required for those resources.
---
▶️ How to Run
Download or clone the repository.
Keep `webpage1.html` and `rtclogo.png` in the same project folder.
Open `webpage1.html` in a modern web browser such as Google Chrome.
Select a state and district.
Choose pickup and drop-off stops from the suggestions.
Select the journey date and preferred time.
Click Search Route & Check Timings to view the sample timetable and route map.
Try the navigation menus to explore profile, enquiry, logistics, food, help, emergency, and complaint interfaces.
An internet connection is needed for externally hosted libraries, map tiles, and route-service requests.
---
⚠️ Current Limitations
No official APSRTC/TGSRTC API integration is included.
No live GPS bus tracking is implemented in this file.
Bus timetable entries are sample/mock data.
Bus-stop data is incomplete demo data and should be verified before real-world use.
Route distance comes from the routing service when available; otherwise, a straight-line fallback is used.
Journey time is an estimate based on an assumed average speed, not actual traffic or RTC operating data.
Seat availability and booking are frontend-only demonstrations and are not shared between users.
Login, referral, enquiry, complaint, and logistics forms show demo interactions; they do not submit data to a backend.
Profile edits are not saved permanently.
The project does not process payments or issue real tickets.
---
🔮 Future Enhancements
Integrate authorized APSRTC and TGSRTC timetable and bus-location APIs.
Add real-time GPS tracking from bus devices.
Show verified arrival predictions and service alerts.
Connect seat inventory to a secure backend database.
Implement user authentication and persistent passenger profiles.
Add real ticket booking and payment integration, if supported by the operator.
Store enquiry, complaint, referral, and logistics requests in a backend.
Add an administrator dashboard for managing routes, stops, schedules, and buses.
Expand and verify district-wise bus-stop coordinates.
---
🎯 Project Objectives
Make bus route information easier for passengers to access.
Help users choose pickup and destination stops.
Present route maps and estimated journey information.
Bring passenger support and travel-related options into one interface.
Demonstrate how web technologies can support public-transport journey planning.
---
👨‍💻 Project Information
Project name: PALLEVELUGU LIVE
Project type: Web application / frontend prototype
Domain: Public transportation and journey planning
Transport focus: APSRTC and TGSRTC
Tagline: KNOW YOUR BUS, PLAN YOUR JOURNEY
---
📄 License
This project is provided for educational and demonstration purposes. Check the terms of any external libraries, map services, images, and data sources before using the project commercially.
---
PALLEVELUGU LIVE — Making bus journey planning easier.