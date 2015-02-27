# VideoScroller.js

## Demo


## Installation

```
npm install video-scroller
```

## Usage

```
new VideoScroller({
    el: document.getElementById('myVideoElement')
});
```

## Options

* `el` video element (required)
* `invert` reverses playback directions / scroll direction,
* `scrollTimeout` how often new position is calculated when scrolling
* `easingFunction` custom easing function, using only one parameter [0-1] and returning [0-1]

## Video requirements

To get the video to scroll smoothly it has to have a generous number of keyframes, here is how you would do that using [ffmpeg](https://www.ffmpeg.org/)

`ffmpeg -i input.mp4 -g 10 output.mp4`