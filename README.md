# IM-AGES: Advanced Image Processing & Analysis Suite 🖼️

[![.NET](https://img.shields.io/badge/.NET-7-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
[![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)](https://docs.microsoft.com/en-us/dotnet/csharp/)
[![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)

**IM-AGES** is a feature-rich desktop application for Windows, engineered with C# and .NET 7 to provide a comprehensive suite of tools for image processing, editing, and analysis. Leveraging the power of the OpenCV library, this application offers both fundamental and advanced functionalities for users ranging from hobbyists to professionals in the field of computer vision.

---

## 📖 Table of Contents

- [📌 About The Project](#-about-the-project)
- [✨ Core Features & Functionality](#-core-features--functionality)
- [🛠️ Built With](#️-built-with)
- [🔬 Technical Deep Dive](#-technical-deep-dive)
- [📂 Project Structure](#-project-structure)
- [🚀 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation Guide](#installation-guide)
- [👥 Meet the Team](#-meet-the-team)
- [🤝 Contributing](#-contributing)

---

## 📌 About The Project

In the world of digital media and data science, the ability to manipulate and analyze images is crucial. IM-AGES was developed to provide a powerful, yet intuitive, desktop solution that centralizes common image processing tasks. Unlike web-based editors that rely on internet connectivity and may have limitations, IM-AGES is a native Windows application that harnesses the full power of the user's machine to perform complex operations quickly and efficiently.

From basic cropping and filtering to advanced histogram analysis, the application serves as an excellent tool for learning, experimentation, and practical use in image-related projects.

---

## ✨ Core Features & Functionality

-   **Main Dashboard (`Ana_Sayfa`):** A central hub that provides access to all the main features of the application.
-   **Advanced Image Editor (`IM_AGES_Edit`):** The core of the application, offering a wide range of editing tools:
    -   **Image Loading & Saving:** Supports various common image formats.
    -   **Cropping:** A dedicated interactive form (`CropForm`) for precise image cropping.
    -   **Rotation & Flipping:** Standard transformation tools.
    -   **Filtering:** Apply various filters to enhance or modify images.
    -   **Color Space Conversion:** Convert images between different color models (e.g., RGB, Grayscale).
-   **Histogram Analysis:** Utilizes the `OxyPlot` library to generate and display color histograms, allowing users to analyze the tonal distribution of an image.
-   **Team/About Section:** Dedicated forms (`Alperen.cs`, `Furkan.cs`, etc.) to showcase the development team behind the project.
-   **Help & Support (`Yardım`):** An integrated help section to guide users through the application's features.

---

## 🛠️ Built With

This project is built on a solid foundation of industry-standard technologies and libraries for Windows desktop development.

-   **Core Framework:** [.NET 7](https://dotnet.microsoft.com/)
-   **Programming Language:** [C#](https://docs.microsoft.com/en-us/dotnet/csharp/)
-   **User Interface:** [Windows Forms (WinForms)](https://docs.microsoft.com/en-us/dotnet/desktop/winforms/)
-   **Image Processing Engine:** [OpenCvSharp](https://github.com/shimat/opencvsharp) (A .NET wrapper for OpenCV)
-   **Data Visualization:** [OxyPlot](https://oxyplot.github.io/) for plotting graphs and histograms.

---

## 🔬 Technical Deep Dive

-   **Computer Vision with OpenCvSharp:** The application's image processing capabilities are powered by OpenCvSharp. This allows for direct access to the highly optimized and extensive OpenCV library. Operations like color conversions, filtering, and geometric transformations are performed efficiently by leveraging native code, which provides a significant performance advantage over managed code alternatives.

-   **Data Plotting with OxyPlot:** To provide analytical insights, the application integrates OxyPlot. When a user requests a histogram, the application first processes the image data (using OpenCV) to calculate the frequency of each pixel intensity for the Red, Green, and Blue channels. This data is then bound to an OxyPlot `PlotModel` to render a clear and interactive histogram chart within a Windows Forms control.

---

## 📂 Project Structure

The project is organized into several key components, ensuring a clean and maintainable codebase.

```
IM-AGES/
├── Properties/             # Project settings and assembly info
├── Resources/              # Image assets and icons for the UI
├── Resimler/               # Sample images for testing
├── bin/
│   └── Debug/              # Compiled application and dependencies
├── Ana_Sayfa.cs            # The main dashboard form
├── IM_AGES_Edit.cs         # The primary image editing form
├── CropForm.cs             # The dedicated image cropping utility
├── Alperen.cs              # Example of a team member "About" form
├── Program.cs              # The main entry point for the application
└── IM-AGES.csproj          # The C# project file defining dependencies and settings
```

---

## 🚀 Getting Started

To set up and run this project locally, please follow the steps below.

### Prerequisites

-   **IDE:** [Visual Studio 2022](https://visualstudio.microsoft.com/) with the ".NET desktop development" workload installed.
-   **.NET SDK:** [.NET 7 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/7)

### Installation Guide

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/IM-AGES.git](https://github.com/your-username/IM-AGES.git)
    cd IM-AGES
    ```

2.  **Open the Project in Visual Studio:**
    -   Launch Visual Studio 2022.
    -   Click on "Open a project or solution".
    -   Navigate to the cloned directory and open the `IM-AGES.csproj` file.

3.  **Restore NuGet Packages:**
    -   Visual Studio should automatically restore the required NuGet packages (like OpenCvSharp and OxyPlot) upon opening the project.
    -   If it doesn't, right-click on the solution in the "Solution Explorer" and select "Restore NuGet Packages".

4.  **Build the Solution:**
    -   From the top menu, go to `Build` > `Build Solution` or press `Ctrl+Shift+B`.

5.  **Run the Application:**
    -   Press `F5` or click the "Start" button in the Visual Studio toolbar to launch the application. The main window (`Ana_Sayfa`) should appear.

---

## 👥 Meet the Team

This application was developed by a dedicated team of individuals. The "About Us" section within the application introduces each member, with dedicated forms for:
-   Alperen
-   Furkan
-   Ismail
-   Mustafa

---

## 🤝 Contributing

Contributions are welcome and greatly appreciated! If you have ideas for new features or improvements, please feel free to contribute.

1.  **Fork** the Project.
2.  Create your Feature Branch (`git checkout -b feature/NewImageEffect`).
3.  Commit your Changes (`git commit -m 'Add some NewImageEffect'`).
4.  Push to the Branch (`git push origin feature/NewImageEffect`).
5.  Open a **Pull Request**.
