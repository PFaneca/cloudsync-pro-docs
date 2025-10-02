# Smart Backup Scheduler
## CloudSync Pro's Intelligent Backup Automation

---

## Product Overview

Smart Backup Scheduler helps small businesses backup their data automatically. No more manual backups or forgotten files.

**Who is this for?**
- Small business owners
- IT managers
- Remote teams

**Why use it?**
- Save money on storage
- Never lose important files
- Backups happen automatically

---

## Features

- Intelligent scheduling during quiet hours
- Custom retention policies (daily, weekly, monthly)
- Email alerts when backups fail
- Faster backups when files change more
- Works with your CloudSync Pro account

---

## Getting Started

### What you need

Before starting:
- CloudSync Pro account (Business plan)
- Admin access
- 10GB free storage

### Step 1: Open the dashboard

1. Login to CloudSync Pro
2. Go to Settings
3. Click Backup & Recovery
4. Enable Smart Backup Scheduler

### Step 2: Create a schedule

1. Click "New Schedule"
2. Give it a name
3. Pick how often (daily, weekly, monthly)
4. Choose the time (2am is good)
5. Select which files to backup
6. Set how long to keep backups
7. Click Save

### Step 3: Test it

> Always test your backup before trusting it!

1. Select your schedule
2. Click "Run Test"
3. Wait 2-5 minutes
4. Check if files backed up correctly

### Step 4: Setup alerts

1. Go to Settings → Notifications
2. Turn on alerts
3. Add your email
4. Choose what alerts you want
5. Save

---

## Configuration Examples

### Simple daily backup

```json
{
  "schedule_name": "Daily Business Hours",
  "frequency": "daily",
  "time": "02:00",
  "retention_days": 30,
  "file_change_threshold": 0.1
}
```

### Weekly backup

```json
{
  "schedule_name": "Weekly Backup",
  "frequency": "weekly",
  "days": ["Sunday"],
  "time": "03:00",
  "retention_days": 90
}
```

---

## API Integration

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/v2/schedules` | GET | List all backup schedules |
| `/api/v2/schedules` | POST | Create new schedule |
| `/api/v2/schedules/{id}/status` | GET | Check schedule status |

### Example request

```bash
curl -X GET https://api.cloudsyncpro.com/api/v2/schedules \
  -H "Authorization: Bearer YOUR_API_KEY"
```

---

## Troubleshooting

### Backup not running

- Check time zone settings
- Make sure app is open
- Verify internet connection

### Not enough storage

- Buy more storage
- Keep backups for less time
- Turn on compression

### Missing files

- Check which folders are selected
- Look at backup logs
- Check file permissions

### No alerts

- Check email address is correct
- Look in spam folder
- Add us to safe senders list

**Need help?**
Email: support@cloudsyncpro.com  
Phone: 1-800-CLOUDSYNC

---

## Support and Resources

### Contact us

- Email: support@cloudsyncpro.com
- Live Chat: Available 24/7
- Phone: 1-800-CLOUDSYNC

### Request a feature

1. Go to feedback.cloudsyncpro.com
2. Search if someone already asked
3. Submit your idea
4. Vote on other ideas

---

## Next Steps

- [ ] Enable Smart Backup Scheduler
- [ ] Create first schedule
- [ ] Test backup
- [ ] Setup alerts
- [ ] Share with team

---

*Last updated: October 2025*
