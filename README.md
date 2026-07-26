# ZeroSight360 LinkedIn Automation

Automated LinkedIn posting for ZeroSight360 via GitHub Actions + Buffer API.

## How It Works

1. **GitHub Actions Cron** triggers at scheduled times
2. **Workflow** reads post data from `posts/posts.json`
3. **Buffer API** publishes the post with image immediately

## Schedule (Week 2: Aug 11-15, 2026)

### Company Page (@zerosight360)
| Date | Time (IST) | Topic | Thumbnail |
|------|------------|-------|-----------|
| Aug 11 | 9:00 AM | Cloud Misconfig | Big Stat (65%) |
| Aug 12 | 9:00 AM | API Security | Split Panel |
| Aug 13 | 9:00 AM | Supply Chain | Checklist |
| Aug 14 | 9:00 AM | Zero-Day | Warning Alert |
| Aug 15 | 9:00 AM | Identity Security | Thread Opener |

### Personal Profile (@nishajiths)
| Date | Time (IST) | Topic | Thumbnail |
|------|------------|-------|-----------|
| Aug 11 | 9:30 AM | S3 Story | Quote Card |
| Aug 12 | 9:30 AM | AI Phishing | Comparison |
| Aug 13 | 9:30 AM | NPM Dependency | Case Study |
| Aug 14 | 9:30 AM | Zero-Day Response | Process Flow |
| Aug 15 | 9:30 AM | AI Code Security | Field Note |

## Setup

### 1. Add Buffer API Key as GitHub Secret
```
Settings → Secrets → Actions → New repository secret
Name: BUFFER_API_KEY
Value: <your-buffer-api-key>
```

### 2. Enable GitHub Actions
The workflows will run automatically on schedule.

### Manual Posting
You can manually trigger any post:
1. Go to Actions → "Post to LinkedIn via Buffer"
2. Click "Run workflow"
3. Enter post ID (e.g., `company_1`, `personal_3`)

## Files

```
├── .github/workflows/
│   └── post-to-linkedin.yml    # GitHub Actions workflow
├── posts/
│   └── posts.json              # All post content + metadata
├── design_01_big_stat.png      # Thumbnail: Cloud Misconfig
├── design_02_split_panel.png   # Thumbnail: API Security
├── design_03_checklist.png     # Thumbnail: Supply Chain
├── design_04_warning.png       # Thumbnail: Zero-Day
├── design_05_quote.png         # Thumbnail: S3 Story
├── design_06_comparison.png    # Thumbnail: AI Phishing
├── design_07_thread.png        # Thumbnail: Identity Security
├── design_08_case_study.png    # Thumbnail: NPM Dependency
├── design_09_process_flow.png  # Thumbnail: Zero-Day Response
└── design_10_field_note.png    # Thumbnail: AI Code Security
```

## Adding New Posts

1. Add thumbnail image to repo root
2. Add post entry to `posts/posts.json`
3. Add cron schedule to `.github/workflows/post-to-linkedin.yml`

## Buffer Channels

| Channel | ID | Type |
|---------|----|----|
| zerosight360 | `6a6484dbe2638b94d7d11e86` | Company Page |
| nishajiths | `6a6484dae2638b94d7d11e85` | Personal Profile |
