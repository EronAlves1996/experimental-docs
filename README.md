# Demonstration Typedoc

## Running

This can be runned just with your favorite browser or by liveserver:

### Option 1: Browser

I use firefox. So I use the following command:

```sh
$ firefox ./index.html
```

### Option 2: Live Server

If you have Live Server installed, you can use it to serve the files for you:

```sh
cd experimental-docs
live-server
```

### Command that generated this docs

As I installed typedoc globally, I used the following command:

```sh
typedoc --entryPointStrategy resolve src/index.ts src/tokens/space.ts src/themes/Bruttal src/tokens/fontSizes.ts src/tokens/fontWeights.ts src/tokens/letterSpacings.ts src/tokens/lineHeights.ts
```

### How it works

With `resolve` as `entryPointStrategy`, every file that you provided as entrypoint will be resolved and produce a single webpage with entrypoint in `index.html`. It proves that can be used with good and flexible configuration.
Also, supports TSDoc. Read more here: https://typedoc.org/guides/overview/
