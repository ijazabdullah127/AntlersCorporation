# Vacation Scheduler Mobile Application

## Title and Purpose
**Vacation Scheduler** is a comprehensive Android mobile application designed for travelers to efficiently track and manage their vacations and associated excursions. The application provides a user-friendly interface to organize travel plans, set reminders, and share vacation details.

## Key Features
- Create, update, and delete vacation entries
- Manage excursions for each vacation
- Date validation and logical constraints
- Smart alerts and notifications
- Share vacation details via email, SMS, or clipboard
- Beautiful Material Design UI
- Offline functionality with Room Database

## Android Compatibility
- **Target Android Version**: Android 8.0 (API level 26) and higher
- **Compiled with**: Android SDK 34
- **Minimum SDK**: API level 26

## How to Operate the Application

### Getting Started
1. Launch the application from your device
2. You'll see the home screen with navigation options

### Managing Vacations
1. **View All Vacations**: Tap "My Vacations" from the home screen
2. **Add New Vacation**:
    - Tap the "+" floating action button
    - Fill in vacation details (title, hotel, start/end dates)
    - Tap "Save Vacation"
3. **Edit Vacation**:
    - Tap on any vacation from the list
    - Modify details and tap "Update Vacation"
4. **Delete Vacation**:
    - Tap on any vacation from the list
    - Press the delete icon from the action bar at the top
    - Confirm deletion (only allowed if no excursions exist)

### Managing Excursions
1. **View Excursions**: Tap on a vacation and then press the location icon from the action bar at the top to see its excursions
2. **Add Excursion**:
    - Tap the "+" button in the excursions list
    - Enter title and date (must be within vacation dates)
    - Tap "Save Excursion"
3. **Edit/Delete Excursions**: Similar process to vacations

### Setting Alerts
1. In vacation or excursion detail view
2. Toggle the "Set Alert" switch
3. Alerts will trigger on specified dates

### Sharing Vacations
1. Open vacation details
2. Tap the share icon
3. Choose sharing method (Email, SMS, or Copy to Clipboard)

## Navigation Flow
```
Home Screen
├── My Vacations (List View)
│   ├── Add Vacation (Detail View)
│   └── Vacation Details
│       ├── Edit Vacation
│       └── Excursions List
│           ├── Add Excursion
│           └── Excursion Details
├── Upcoming Alerts
└── App Settings
```

## Validation Rules
- Start date must be before end date for vacations
- Excursion dates must fall within the vacation period
- All dates must be properly formatted
- Vacation titles and hotel names are required
- Vacations with excursions cannot be deleted

## Technical Specifications
- **Database**: Room Framework with SQLite
- **Architecture**: MVVM with LiveData
- **UI Framework**: Material Design Components
- **Date Handling**: Modern DatePicker with validation
- **Notifications**: Android Notification System
- **Sharing**: Android Intent System

## Installation Instructions
1. Download the provided APK file
2. Enable "Install from Unknown Sources" in your device settings
3. Install the APK file
4. Launch the application

## Git Repository
[Repository Link: https://github.com/yourusername/vacation-scheduler]

## Development Notes
- Built with Android Studio
- Uses Gradle build system
- Implements proper error handling and user feedback
- Follows Android development best practices
- Responsive design for various screen sizes

