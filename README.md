# morningcheckin
Home Assistant "no movement" check-in with motion sensor

Morning Check-In Safety System
A simple, privacy-first Home Assistant automation that monitors morning activity using a motion sensor and alerts designated contacts if no motion is detected during a scheduled time window.
Overview
This system is designed for people who live alone or want an extra layer of safety. If no motion is detected during a configurable morning window, designated friends or family members automatically receive a push notification suggesting they check in. All automations and data run locally on the user's own Home Assistant server. Remote dashboard access for contacts uses an encrypted Home Assistant Cloud connection, but no data is stored externally.
Features

Motion-based check-in monitoring
Configurable daily time window via the dashboard
Automatic push notifications to designated contacts
Fully local — no cloud dependency
Simple dashboard interface for non-technical users

Current Status
This is a working MVP (minimum viable product). The core functionality — motion detection, scheduling, and push notifications — works as intended.
Known Limitations

Adding friends/contacts currently requires manual entry in the YAML configuration
No invitation or permission flow exists for contacts being added
Passwords for contacts are currently set manually by the system owner

Future Development Goals
The main goal is to make this system accessible to non-technical users by adding:

A setup wizard for adding contacts without coding
An invitation flow so contacts can accept and set their own credentials
Better onboarding for anyone wanting to deploy this system themselves

Files

configuration.yaml — defines system components and input helpers
automations.yaml — core automation logic
templates.yaml — template sensors (if applicable)

Contributing
This is an open project and help is welcome! If you have experience with Home Assistant and are interested in contributing — particularly around the contact onboarding flow — please open an issue or reach out via the Home Assistant Community Forums.
