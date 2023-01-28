<div id="header" align="center">
  <img src="https://media.giphy.com/media/bfCRQtWUmduWBkDpL7/giphy.gif" width="100"/>
</div>

I'm Sergei Beliaev, a back-end developer from Russia. I love to explore and learn about new things...


[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=scyberlife&theme=synthwave)](https://git.io/streak-stats)

name: Latest blog post workflow on: schedule: # Runs every hour - cron: '0 * * * *' workflow_dispatch:

jobs: update-readme-with-blog: name: Update this repos README with latest blog posts runs-on: ubuntu-latest steps: - uses: actions/checkout@v2 - uses: gautamkrishnar/blog-post-workflow@master with: max_post_count: "4" feed_list: "https://dev.to/feed/itszed0"
