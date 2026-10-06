SpendWise Dashboard
Project Description

SpendWise is a responsive personal finance dashboard shell built using HTML and CSS. The project provides the visual foundation for a personal finance application.

The dashboard contains a navigation sidebar, header, financial summary cards, expense category cards, and recent transactions.

The project uses static financial information because functionality is not required for this assignment.

Dashboard Sections
Sidebar

The sidebar contains the SpendWise logo and navigation links for:

Dashboard

Income

Expenses

Budgets

Savings

Settings

Flexbox is used to arrange the navigation items.

Header

The header contains a welcome message and user profile information.

Flexbox is used to arrange the header content.

Financial Summary

The summary section displays:

Total Balance

Monthly Income

Monthly Expenses

CSS Grid is used to arrange these summary cards.

Expense Categories

The dashboard contains six expense categories:

Food

Transport

Rent

Entertainment

Savings

Utilities

CSS Grid is used to arrange the category cards, while Flexbox is used inside each card.

Recent Transactions

The transactions section displays realistic static financial transactions such as supermarket purchases, fuel expenses, and salary income.

Flexbox is used to arrange the transaction information.

CSS Grid

CSS Grid is used for the main dashboard layout and card sections.

The main dashboard uses two columns on larger screens:

.dashboard {
    display: grid;
    grid-template-columns: 240px 1fr;
}


The expense cards also use CSS Grid.

Flexbox

Flexbox is used inside the dashboard components.

It is used for:

Sidebar navigation

Header

User profile

Dashboard cards

Category cards

Transaction items

CSS Custom Properties

The project uses CSS custom properties to create a consistent color theme.

The variables are defined inside :root and include:

Brand color

Accent color

Background color

Surface color

Primary text color

Secondary text color

This makes the colors easier to maintain and change.

Responsive Design

A media query is used at 768px.

Below 768px, the dashboard changes to a single-column layout.

The category cards and summary cards also stack vertically to make the dashboard easier to use on smaller screens.

The responsive layout can be tested using the browser's DevTools Device Toolbar.

Card Micro-interactions

The expense category cards have hover and keyboard focus effects.

When a user hovers over or focuses on a card, the card moves slightly upward and receives a shadow.

The transition lasts 200ms, which is within the required maximum of 250ms.

The cards use tabindex="0" so that they can receive keyboard focus.

Dark Theme

The project includes a dark theme using:

@media (prefers-color-scheme: dark)


The dark theme works by overriding the CSS custom properties defined in :root.

Technologies Used

HTML5

CSS3

CSS Grid

CSS Flexbox

CSS Custom Properties

CSS Media Queries

Project Files
spendwise-dashboard/
├── index.html
├── style.css
└── README.md

Testing

The dashboard should be tested using the browser's Developer Tools Device Toolbar.

The responsive layout should be checked at different screen sizes, especially below 768px.

Keyboard navigation can also be tested using the Tab key to confirm that the dashboard cards receive focus.
