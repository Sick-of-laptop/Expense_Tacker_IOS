# Expense Tracker

A comprehensive iOS expense tracking application built with Swift and Xcode. Track your daily spending, categorize expenses, and visualize your financial habits with an intuitive and user-friendly interface.

## 📋 Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

- **Add & Manage Expenses**: Easily record new expenses with details like amount, category, date, and notes
- **Categorized Tracking**: Organize expenses by predefined categories (Food, Transportation, Entertainment, Utilities, etc.)
- **Dashboard Overview**: View spending summary at a glance
- **Date-based Organization**: Filter and view expenses by date range
- **Edit & Delete**: Modify or remove expense entries as needed
- **Search Functionality**: Quickly find specific expenses
- **Visual Analytics**: Charts and graphs to visualize spending patterns
- **Local Storage**: All data stored securely on device using Core Data or UserDefaults
- **Clean UI**: Intuitive and responsive user interface built with SwiftUI or UIKit

## 📱 Requirements

- **iOS**: 14.0 or later
- **Xcode**: 13.0 or later
- **Swift**: 5.5 or later
- **Device**: iPhone (supports various screen sizes)

## 🚀 Installation

### Clone the Repository

```bash
git clone https://github.com/Sick-of-laptop/Ios_project.git
cd Ios_project
```

### Open in Xcode

1. Launch Xcode
2. Select **File → Open**
3. Navigate to the cloned project folder
4. Select the `.xcodeproj` or `.xcworkspace` file
5. Click **Open**

### Build & Run

1. Select your target device or simulator from the device dropdown
2. Press **Cmd + R** or click the **Run** button
3. The app will build and launch on your selected device

## 🎯 Getting Started

### First Launch

1. Grant necessary permissions (if applicable)
2. Start by tapping the **"+" button** to add a new expense
3. Fill in the expense details:
   - **Amount**: Enter the spending amount
   - **Category**: Select from available categories
   - **Date**: Choose the transaction date
   - **Description**: Add optional notes (optional)
4. Tap **Save** to record the expense

### Managing Expenses

- **View All**: Scroll through your expense list on the home screen
- **Filter by Date**: Use date pickers to filter expenses by time period
- **Edit**: Tap on an expense and modify its details
- **Delete**: Swipe or long-press to remove an expense
- **Search**: Use the search bar to find specific transactions

## 📁 Project Structure

```
Ios_project/
├── Models/
│   └── Expense.swift
├── Views/
│   ├── ContentView.swift
│   ├── AddExpenseView.swift
│   ├── ExpenseDetailView.swift
│   └── ChartView.swift
├── ViewModels/
│   └── ExpenseViewModel.swift
├── Services/
│   └── DataManager.swift
├── Assets/
│   └── Assets.xcassets/
├── Info.plist
└── Ios_projectApp.swift
```

## 💡 Usage Examples

### Adding an Expense

```swift
let expense = Expense(
    id: UUID(),
    amount: 25.50,
    category: "Food",
    date: Date(),
    description: "Lunch at cafe"
)
expenseManager.addExpense(expense)
```

### Fetching Expenses

```swift
let allExpenses = expenseManager.getAllExpenses()
let monthlyExpenses = expenseManager.getExpensesByMonth(Date())
let categoryTotal = expenseManager.getTotalByCategory("Food")
```

## 🏗️ Architecture

The application follows the **MVVM (Model-View-ViewModel)** architecture pattern:

- **Model**: `Expense` class containing expense data
- **View**: SwiftUI views for UI presentation
- **ViewModel**: `ExpenseViewModel` managing business logic and state
- **Service**: Data persistence layer handling Core Data or file storage

## 🛠️ Technologies Used

- **Language**: Swift 5.5+
- **UI Framework**: SwiftUI / UIKit
- **Data Persistence**: Core Data / UserDefaults
- **Development Environment**: Xcode 13+
- **Architecture Pattern**: MVVM
- **iOS Version**: iOS 14.0+

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the MIT License. See the LICENSE file for more details.

---

## 📞 Support & Contact

For issues, questions, or suggestions, please open an issue on the [GitHub Issues](https://github.com/Sick-of-laptop/Ios_project/issues) page.

**Happy Tracking! 💰**
