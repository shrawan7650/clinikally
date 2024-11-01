
# DeliveryAppChainkinsDemo

A React Native app for delivery estimation based on product selection and pincode input. The app calculates same-day, next-day, and general delivery dates using logistics provider rules and stock availability.

## Setup Instructions

1. **Prerequisites**: Install [Node.js and npm](https://nodejs.org/), [Expo CLI](https://docs.expo.dev/get-started/installation/).
2. **Installation**:
   ```bash
   https://github.com/shrawan7650/clinikally.git
   cd clinikally
   npm install
   ```
3. **Run the App**:
   ```bash
   npx expo start
   ```
4. **Web Deployment** (optional): For web, install `react-native-web` and run `npm start`.

## Assumptions

- **Stock Simulation**: 80% of products in stock.
- **Pincode Mapping**: Predefined provider mapping.
- **Delivery Rules**:
  - **Provider A**: Same-day before 5 PM.
  - **Provider B**: Same-day before 9 AM; next-day otherwise.
  - **General Partners**: 2-5 day delivery based on region.
- **Countdown Timer**: Shows cutoff time for Providers A and B.

## Key Design Decisions

1. **Component-Based UI**: Divides UI into reusable components like `ProductList`, `ProductCard`, `ProductCardDetials`, and `DeliveryEstimator`.
2. **Data-Driven Logic**: Caching and simulated data for 5000 products and 25,000 pincodes.
3. **Delivery Logic with `date-fns`**: Handles same-day/next-day rules using date functions.
4. **Responsive UI**: Designed for both mobile and web use.

## Features

- **Product Selection**: Choose a product to check stock.
- **Pincode Validation**: Validate pincodes for logistics mapping.
- **Delivery Estimation**: Calculate delivery dates based on rules.
- **Countdown Timer**: For same-day cutoff visibility.
  
## Project Structure

```
/DeliveryAppChainkinsDemo
├── /components          # UI Components
├── /screens             # Main Screens
├── App.js               # Entry point
├── /utils               # Delivery logic
└── README.md            # Documentation
```
![WhatsApp Image 2024-10-27 at 19 34 05_7df92f72](https://github.com/user-attachments/assets/0e08eb53-5d01-4012-8232-2d1063dc6706)
![WhatsApp Image 2024-10-27 at 19 34 05_725bbfa3](https://github.com/user-attachments/assets/ef5a40cd-eb84-4573-b883-30cf562703bf)
![WhatsApp Image 2024-10-27 at 19 34 06_07a0307f](https://github.com/user-attachments/assets/541fdbc1-3e6f-4250-9950-3ddde9d18843)
![WhatsApp Image 2024-10-27 at 19 34 06_b586b7bc](https://github.com/user-attachments/assets/4536390f-ef9e-4493-a93d-7ec707af37d0)


