# about

updates [`blockheight.json`](./blockheight.json) every 15 minutes with the current bitcoin blockheight

data comes from [mempool.space's api](https://mempool.space/docs/api/rest#get-block-tip-height)

updates happen via via a cron job in the [github action workflow](./.github/workflows/update-blockheight.yml)

primarmily using this for my [TRMNL](https://usetrmnl.com?ref=tyler) e-ink display. see [that plugin repo](https://github.com/tyler-dot-earth/trmnl-notblockclock) if interested.

# how to run your own

- create github repo
- settings > actions > general > enable read/write for workflows
    - this lets the action do the commit
- use [the json file](./blockheight.json)'s raw json

# acknowledgements

- [mempool.space](https://mempool.space/)
- [mempool.space's api](https://mempool.space/docs/api/rest#get-block-tip-height)
- [github actions](https://github.com/features/actions)
- [lucide icons](https://lucide.dev/)
