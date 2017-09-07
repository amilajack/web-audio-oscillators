# web-audio-oscillators [![NPM version](http://img.shields.io/npm/v/web-audio-oscillators.svg?style=flat-square)](https://www.npmjs.org/package/web-audio-oscillators)

A collection of custom oscillators for use with the [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API).

## Installation

Install the package with NPM:

```bash
$ npm install web-audio-oscillators
```

## Usage

For example, to create an [OscillatorNode](https://developer.mozilla.org/en-US/docs/Web/API/OscillatorNode) that sounds like an organ:

```javascript
import oscillators from "web-audio-oscillators";

let context = new (window.AudioContext || window.webkitAudioContext)();
let oscillator = oscillators.organ(context);
oscillator.frequency.value = 220;
oscillator.connect(context.destination);
oscillator.start();
```

All oscillators provided by this package:

- `sine`
- `square`
- `square2`
- `sawtooth`
- `triangle`
- `triangle2`
- `chiptune`
- `organ`
- `organ2`
- `organ3`
- `organ4`
- `bass`
- `bass2`
- `bass3`
- `bass4`
- `brass`
- `brass2`
- `choirAah`
- `choirOoh`
- `choirEeh`
- `buzz`
- `buzz2`
- `dissonance`

## Contributing

Pull requests are most welcome. I'd like to expand this collection in order to cover more musical scenarios.
