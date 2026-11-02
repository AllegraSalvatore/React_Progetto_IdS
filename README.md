# CSV Explorer
### Explore your data. Find what matters.

<p align="center">
  <strong>A simple and intuitive way to explore, filter and export CSV datasets.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-Frontend-61DAFB?logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Architecture-MVC-8B5CF6" />
  <img src="https://img.shields.io/badge/Bootstrap-4.6-7952B3?logo=bootstrap&logoColor=white" />
</p>

---

## 📌 Overview

**CSV Explorer** is a web application developed with React that makes working with CSV files easier and more efficient.

It provides an intuitive interface to upload datasets, explore tabular information, perform targeted searches, customize displayed columns and export filtered results.

Whether you need to find a specific value, inspect selected fields or extract a subset of your data, CSV Explorer brings everything together in one simple workspace.

<p align="center">
  <img src="https://placehold.co/1000x480/101827/FFFFFF?text=CSV+Explorer%7C+Explore+your+data" alt="CSV Explorer application preview" width="90%" />
</p>

---

## ✨ Key Features

<table>
<tr>
<td width="50%" valign="top">

### 📂 CSV Upload

Import CSV files directly into the application and start exploring their contents.

</td>
<td width="50%" valign="top">

### 📊 Interactive Data Table

Display CSV contents in a structured table for easier data consultation.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔎 Advanced Search

Search for values across entire rows or within specific columns.

</td>
<td width="50%" valign="top">

### 🎛️ Column Management

Choose which columns to display and customize your working view.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔍 Combined Filtering

Combine row-based and column-based searches to narrow down results.

</td>
<td width="50%" valign="top">

### 📤 CSV Export

Download the resulting dataset, including selected columns and filtered rows.

</td>
</tr>
</table>

---

## 🚀 How It Works

A straightforward workflow designed to make CSV exploration effortless.

```mermaid
flowchart TD
    A["📂 Upload CSV File"] --> B["📊 Display Dataset"]
    B --> C["🔎 Search and Filter"]
    C --> D["🎛️ Select Columns"]
    D --> E["📤 Export Results"]

    style A fill:#DBEAFE,stroke:#2563EB,color:#1E3A8A
    style B fill:#E0E7FF,stroke:#4F46E5,color:#312E81
    style C fill:#EDE9FE,stroke:#7C3AED,color:#4C1D95
    style D fill:#FCE7F3,stroke:#DB2777,color:#831843
    style E fill:#DCFCE7,stroke:#16A34A,color:#14532D
```

### 01 — Upload your dataset

Select a CSV file and load its contents into the application.

### 02 — Explore the information

Browse the dataset through a structured tabular interface.

### 03 — Find what you need

Use two different search modes:

- **Row Search:** find rows containing a specific value.
- **Column Search:** search for a value within a selected column.

Search criteria can be combined to obtain more specific results.

### 04 — Customize your workspace

Select the columns you want to display and hide unnecessary information.

### 05 — Export your results

Generate a new CSV file containing the selected columns and the resulting rows after applying your search criteria.

---

## 🏗️ Architecture

CSV Explorer follows the **Model-View-Controller (MVC)** architectural pattern.

The application separates data management, application logic and user interface responsibilities.

```mermaid
flowchart TB
    USER["👤 USER"]

    subgraph VIEW["VIEW"]
        UI["React Components"]
        TABLE["Data Table"]
        SEARCH["Search Interface"]
        COLUMNS["Column Selection"]
    end

    subgraph CONTROLLER["CONTROLLER"]
        LOGIC["Application Logic"]
        FILTER["Search and Filtering"]
        EXPORT["Export Coordination"]
    end

    subgraph MODEL["MODEL"]
        CSV["CSV Data Management"]
        DATA["Dataset Representation"]
    end

    USER --> UI
    UI --> LOGIC
    LOGIC --> CSV
    CSV --> DATA
    DATA --> LOGIC
    LOGIC --> FILTER
    FILTER --> TABLE
    LOGIC --> COLUMNS
    LOGIC --> EXPORT
    EXPORT --> USER

    style VIEW fill:#DBEAFE,stroke:#2563EB,color:#1E3A8A
    style CONTROLLER fill:#EDE9FE,stroke:#7C3AED,color:#4C1D95
    style MODEL fill:#DCFCE7,stroke:#16A34A,color:#14532D
```

### Architectural Responsibilities

| Component | Responsibility |
|---|---|
| **Model** | Manages CSV data and its representation. |
| **View** | Displays the application interface and dataset. |
| **Controller** | Coordinates application operations, searches, filtering and interactions. |

This separation promotes modularity, maintainability and a clearer organization of the application.

---

## 🛠️ Technology Stack

The project combines frontend development tools and libraries.

| Technology | Purpose |
|---|---|
| React | User interface development |
| JavaScript | Application logic |
| Bootstrap 4.6 | Responsive interface styling |
| React Bootstrap Table 2 | Tabular data presentation |
| CSS | Interface customization |

---

## ⚙️ Getting Started

Follow these steps to run the application locally.

### Prerequisites

Make sure you have installed:

- [Node.js](https://nodejs.org/)
- npm (included with Node.js)
- Git

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/AllegraSalvatore/React_Progetto_IdS.git
```

**2. Navigate to the project directory**

```bash
cd React_Progetto_IdS
```

**3. Install dependencies**

```bash
npm install
```

**4. Start the development server**

```bash
npm start
```

Open the local address displayed in your terminal to access the application.

---

## 📁 Project Structure

```text
React_Progetto_IdS/
│
├── public/
│
├── src/
│
├── OBIB(1).csv
│
├── package.json
├── package-lock.json
└── README.md
```

---

## 🎯 Project Vision

CSV Explorer is designed to make CSV data exploration simple, intuitive and efficient.

By combining data visualization, flexible search capabilities and customizable column management, the application provides a straightforward workspace for working with tabular datasets.

Its main goals are:

- Simplify CSV file exploration.
- Make information easier to find through flexible search tools.
- Provide control over displayed data and columns.
- Enable the export of customized datasets.
- Deliver an intuitive and accessible user experience.

---

## 👩‍💻 Author

**Allegra Salvatore**

---

<p align="center">
  <strong>CSV Explorer</strong>
  <br />
  <a href="https://github.com/AllegraSalvatore/React_Progetto_IdS">View Repository</a>
</p>
