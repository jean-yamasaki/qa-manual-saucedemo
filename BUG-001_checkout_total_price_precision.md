[Checkout] Total price shows floating-point precision error with specific product combinations

ID: BUG-001

Environment
Application: SauceDemo
URL: www.saucedemo.com
Browser: Firefox
OS: Windows 11
User type: standard_user, visual_user, performance_glitch_user

Severity: High

Priority: P2

Description
During checkout, the site shows a floating-point precision error when specific product combinations are added to the cart.

Steps to reproduce
1. Log in as standard_user
2. Add Sauce Labs Fleece Jacket to the cart
3. Add Sauce Labs Onesie or Sauce Labs Bike Light to the cart
4. Go to checkout
5. Observe the total price

Expected Result
The price should be calculated and displayed correctly, without precision errors. (59.98 OR 57.98)

Actual Result
Total price is displayed as 59.980000000000004 or 57.980000000000004.

Reproducibility
Always with specific product combinations.

Notes
Happens with standard_user, visual_user, performance_glitch_user
Does not happen with other tested product combinations
Appears to be value specific, not order specific

Attachments
BUG-001_checkout_total_precision
BUG-001_checkout_total_precision_2

Status
New