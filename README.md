# ControleAcademico

Android app for tracking absences, grades, and tasks

## Overview

`ControleAcademico` is an Android application designed for students to manage and track their academic records: attendance, grades, and tasks (homework, assignments, etc.). It provides an organized view of subjects, tasks by subject, and simple reporting tools to help students monitor their progress.

## Key Features

- Track attendance (absences) per subject
- Record and calculate grades
- Create, edit, and list tasks (Tarefas) for subjects
- Simple graphical summaries for quick visualization
- Local database storage (SQLite)

## Project Structure

- `app/` — Android app module
- `app/src/main/java/br/ufop/ControleAcademico/` — main source package containing activities, models, adapters, and database connection
- `app/src/main/res/` — resources (layouts, drawables, menus, values)

## Requirements

- Android Studio (recommended) or Gradle
- Java / Android SDK matching the project's `compileSdk` and `targetSdk` (open the project in Android Studio to sync)
- `adb` (for installing and testing on devices)

Note: The repository contains `app/google-services.json`. If you replace Firebase or use your own Firebase project, update or replace that file accordingly.

## Build and Run

Open the project in Android Studio and run on an emulator or connected device.

Or build from the command line with the Gradle wrapper:

```bash
./gradlew assembleDebug
./gradlew installDebug
```

Then run the app on a connected device or emulator. To run unit tests (if any):

```bash
./gradlew test
```

## Configuration

- Firebase / Google services configuration lives in `app/google-services.json` if used for notifications or analytics.
- Database initialization is handled by `app/src/main/java/br/ufop/ControleAcademico/connection/Database.java`.

## Contributing

Contributions are welcome. Suggested steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Implement and test your changes
4. Submit a pull request with a clear description of changes

Please follow the existing code style and keep commits focused and well-described.

## License

This project includes a `LICENSE` file in the repository root. Review it for license terms.

## Contact

If you need help or want to report issues, open an issue in this repository or contact the maintainers.
