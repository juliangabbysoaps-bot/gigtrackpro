# GIG Track Pro Testing Guide

## Setup Instructions
1. **Clone the Repository**  
   Clone the gigtrackpro repository to your local machine using the following command:  
   ```bash  
   git clone https://github.com/yourusername/gigtrackpro.git  
   ```

2. **Install Dependencies**  
   Navigate to the project directory and install the necessary dependencies:  
   ```bash  
   cd gigtrackpro  
   npm install  
   ```

3. **Configure Environment Variables**  
   Create a `.env` file in the root of the project using the template provided:  
   ```bash  
   cp .env.example .env  
   ```  
   Populate the `.env` file with your configuration settings.

## Test Scenarios
### 1. User Registration  
- **Scenario**: A new user registers on the platform.  
- **Expected Outcome**: User should receive a confirmation email, and their details should be stored in the database.

### 2. User Login  
- **Scenario**: A registered user attempts to log in.  
- **Expected Outcome**: User successfully logs in and is redirected to the dashboard.

### 3. Create a Gig  
- **Scenario**: A user creates a new gig.  
- **Expected Outcome**: The gig appears in the user's list of gigs and is accessible to others.

### 4. Edit a Gig  
- **Scenario**: A user edits an existing gig.  
- **Expected Outcome**: The updates are reflected in the gig details.

### 5. Delete a Gig  
- **Scenario**: A user deletes a gig.  
- **Expected Outcome**: The gig is removed from the user's list and is no longer accessible.

## Troubleshooting Steps
- **Issue**: Unable to log in.  
  - **Solution**: Check if the correct username and password are being used. Reset the password if necessary.
- **Issue**: Gig not appearing after creation.  
  - **Solution**: Ensure that all required fields are filled in correctly. Check for error messages during the creation process.  
- **Issue**: Unable to send confirmation email.  
  - **Solution**: Verify the email configuration in the .env file.; check the email service provider status.

## Conclusion
This guide serves as a foundational document for testing the GIG Track Pro application. Ensure all scenarios are covered thoroughly to maintain application integrity.