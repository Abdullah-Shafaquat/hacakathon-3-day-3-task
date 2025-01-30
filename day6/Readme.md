# Day 6 - Deployment Preparation and Staging

## Objective
Today, I focused on preparing my marketplace for the live environment by setting up a staging environment and configuring hosting platforms. This is to ensure everything runs smoothly and is ready for customers. I also worked on managing different environments (development, testing, and production) to ensure reliability.

---

## Step 1: Hosting Platform Setup

### 1. Choose a Platform
- **Platform:** Vercel (for deployment) & GitHub (for version control)
- **Reasoning:** Vercel is fast, user-friendly, and ideal for quick deployments. GitHub helps with code management and collaboration. Future configurations may explore AWS or Azure if needed.

### 2. Connect Repository
- Connected GitHub repo to Vercel for automatic deployment.
- Configured build settings and scripts for smooth deployment.

---

## Step 2: Configure Environment Variables

### 1. Create a `.env` File
- Added sensitive variables such as API keys and tokens.

### 2. Upload Variables to Hosting Platform
- Used Vercel’s dashboard to securely add environment variables.

---

## Step 3: Deploy to Staging

### 1. Deploy Application
- Logged into Vercel and selected the GitHub repository.
- Initiated the build process to deploy the app to a staging environment.

### 2. Validate Deployment
- Checked Vercel deployment logs for errors.
- Verified staging environment by testing:
  - Page loads correctly
  - Key features (user login, product listings, search) work
  - No broken links or missing assets.

---

## Step 4: Staging Environment Testing

### 1. Testing
- Functional Testing: Ensured core features work as expected.
- Security Testing: Verified app security measures are in place.
- API Testing: Checked API endpoints for correct responses.

### 2. Performance Testing
- Assessed application performance under different conditions.

### 3. Test Case Reporting
- Documented all test cases and results.
- 
| Test Case ID | Test Case Description                | Test Steps                                            | Expected Result                                          | Actual Result                                          | Status | Severity Level | Assigned To | Remarks                 |
|--------------|--------------------------------------|-------------------------------------------------------|---------------------------------------------------------|-------------------------------------------------------|--------|-----------------|-------------|-------------------------|
| TC001        | Validate car listing page           | Open car listing page > Verify cars                   | Cars displayed correctly with details (name, price, image) | Cars displayed correctly                               | Passed | High            | -           | No issues found         |
| TC002        | Test API error handling             | Disconnect API > Refresh page                         | Show fallback UI with error message                     | Error message shown                                    | Passed | Medium          | -           | Handled gracefully      |
| TC003        | Ensure responsiveness on mobile     | Resize browser window > Check layout                  | Layout adjusts properly to screen size                   | Responsive layout working as intended                 | Passed | Medium          | -           | Test successful         |
| TC004        | Test dynamic routing for car details | Click on car > Verify car details page                | Car details page loads correctly with accurate information (name, price, features) | Car details page loaded correctly                      | Passed | High            | -           | No issues found         |
| TC005        | Validate search and filter          | Use search bar and filters (e.g., by brand, seats) > Verify results | Filters and search return accurate car results          | Filters and search worked as expected                  | Passed | Medium          | -           | Test successful         |
| TC006        | Test API response                   | Use Postman to test GET /api/cars endpoint            | API returns valid response with correct car data         | API returned expected data                            | Passed | High            | -           | No issues found         |
| TC007        | Check fallback UI for empty data    | Simulate empty car list > Verify fallback message     | Fallback message (e.g.,"No cars available") displayed    | Fallback message displayed correctly                   | Passed | Medium          | -           | Handled gracefully      |
| TC008        | Test performance optimization       | Run Lighthouse analysis > Verify load time and performance metrics | Initial load time under 2 seconds                        | Load time improved to under 2 seconds                  | Passed | Medium          | -           | Performance optimized  |
| TC009        | Cross-browser compatibility         | Test website on Chrome, Firefox, and Edge             | Consistent rendering and functionality across all browsers | Website rendered consistently across browsers          | Passed | Medium          | -           | No issues found         |
| TC010        | Test responsive design on devices   | Use BrowserStack and physical device to test responsiveness | Website adjusts seamlessly across all device sizes and orientations | Responsive design worked as intended                  | Passed | High            | -           | Test successful         |
| TC011        | Validate input sanitization         | Attempt SQL injection or XSS attack > Verify input validation | Inputs sanitized to prevent attacks                     | Inputs sanitized successfully                         | Passed | Critical        | -           | Security measures working|
| TC012        | Test secure API communication       | Verify API calls are made over HTTPS                   | API calls are secure and use HTTPS                       | API calls made over HTTPS                             | Passed | High            | -           | No issues found         |
| TC013        | Simulate real-world usage           | Browse cars, rent a car, and checkout                 | All functionalities work as expected                     | All functionalities worked as expected                 | Passed | High            | -           | Test successful         |
| TC014        | Collect user feedback               | Gather feedback from friends and family               | Feedback collected for improvements                      | Feedback collected and documented                      | Passed | Low             | -           | Suggestions noted       |
| TC015        | Fix URL path issue                  | Update URL structure for dynamic routing              | Dynamic routing works correctly                          | Dynamic routing fixed and working                     | Passed | Medium          | -           | Issue resolved          |
| TC016        | Resolve image source error          | Configure external image domain in next.config.ts      | External images load correctly                           | External images loaded successfully                    | Passed | Medium          | -           | Issue resolved          |

---


---

## Step 5: Documentation Updates

### 1. Create README.md
- Summarized all activities, including deployment steps and testing results.

### 2. Organize Project Files
- Ensured all project files from Days 1 to 6 are structured in a clear folder hierarchy.

---

## Checklist for Day 6
- [x] Deployment Preparation
- [x] Staging Environment Testing
- [x] Documentation Updates
- [x] Form Submission
- [x] Final Review

---

## Conclusion

Day 6 marked a crucial step towards launching the marketplace by setting up a staging environment and ensuring everything is functioning properly. The deployment process went smoothly with the integration of Vercel and GitHub. The staging environment allowed for effective testing of functionality, security, and performance. By the end of the day, all key features were verified, and the environment was ready for further testing or final deployment. With the proper organization of files and documentation, the project is on track to go live soon, ensuring a seamless experience for customers.
