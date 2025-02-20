zephyr-module-sync
==================

This repository contains GitHub Actions to synchronize a Zephyr module with its upstream counterpart.
This repository is needed because GitHub does not recognize some of the modules as "official" forks.

There is a form for requesting reattachment of a forked repository, but due to an internal GitHub
implementation detail called "network," reattachment cannot be done if two repositories are not part
of the same network. This repository works around this limitation to reduce the burden of performing manual syncs.

Adding the actions to each module separately is not an option because scheduled action runs are only possible on
the main branch, which would deviate from any upstream syncing efforts.
