# Docker Demo Application
This is a Go demo application used for demonstrating Docker and load balancing.

## Environment Variables

- `TITLE`: sets title in demo app
- `SHOW_VERSION`: show version of app in ui (`VERSION` env var)
- `REFRESH_INTERVAL`: interval in milliseconds for page to refresh (default: 1000)
- `EXPIRE_INTERVAL`: how long a replica can go without being seen before we remove it from the display (default: `REFRESH_INTERVAL` * 5)
- `SKIP_ERRORS`: set this to prevent errors from counting (useful on janky load balancers)
- `METADATA`: extra text at bottom of info area
- `COW_COLOR`: what color the cow background should be (default: black). Valid options are any color from the CSS pallete, including:
  - red
  - orange
  - yellow
  - olive
  - green
  - teal
  - blue
  - violet
  - purple
  - pink
  - black

## Build

`docker build -t monachus/rancher-demo .`
