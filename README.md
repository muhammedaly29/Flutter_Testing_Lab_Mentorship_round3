# Flutter Testing Assignment – Week 4

This project demonstrates three Flutter widgets built with clean architecture, separation of concerns, and proper unit & widget testing.  
It focuses on writing maintainable, testable, and production-ready Flutter UI components.

---

## 🚀 Widgets Overview

### 🧱 1. User Registration Form
A complete registration form that includes:
- Form validation for name, email, password, and password confirmation.
- Validation logic extracted into a separate file for reusability and testability.
- Loading indicator during API simulation.
- Success message display after form submission.

**Key Features**
- Custom validators for clean error handling.
- Clear UI feedback for users (loading + success).
- Unit tests for:
  - Email validation
  - Password strength
  - Empty fields handling

---

### 🛒 2. Shopping Cart
A dynamic shopping cart widget that manages products, quantities, and discounts with accurate calculations.

**Key Fixes & Features**
- Prevents item duplication (increments quantity instead).
- Corrected subtotal, discount, and total calculations.
- Clear cart and item removal functionality.
- Edge case handling for empty carts and 100% discount.
- Business logic covered by unit tests.

**Test Coverage**
- Add / Remove Item
- Clear Cart
- Quantity updates
- Discount calculations

---

### 🌤️ 3. Weather Display
A weather display widget simulating an API call with loading and error states.

**Enhancements**
- Fixed Celsius ↔ Fahrenheit conversion formulas.
- Added robust null and malformed data handling.
- Improved loading and error UI states.
- Extracted `WeatherData` model & conversion logic into `utils/weather_utils.dart`.
- Dependency injection for API fetcher to enable widget testing.

**Testing**
- ✅ Unit tests for:
  - Conversion helpers
  - JSON parsing
  - Exception handling
- ✅ Widget tests for:
  - Loading state
  - Success state
  - Error state
