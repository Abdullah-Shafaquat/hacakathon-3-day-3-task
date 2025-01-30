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
