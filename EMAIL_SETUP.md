# Email Configuration for IUMS

## Setting up Gmail SMTP

### Option 1: Using Streamlit Secrets (Recommended for Deployment)

1. Go to your Gmail account settings
2. Enable 2-factor authentication
3. Generate an App Password:
   - Go to Google Account settings
   - Security → 2-Step Verification → App passwords
   - Generate a password for "Mail"
   - Copy the 16-character password

4. In Streamlit Cloud, add these secrets in your app settings:

```toml
[email]
username = "your.email@gmail.com"
password = "your_16_character_app_password"