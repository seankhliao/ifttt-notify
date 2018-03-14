# ifttt-notify [![GoDoc](https://godoc.org/github.com/seankhliao/ifttt-notify?status.svg)](https://godoc.org/github.com/seankhliao/ifttt-notify) [![Build Status](https://img.shields.io/travis/seankhliao/ifttt-notify.svg?style=flat-square)](https://travis-ci.org/seankhliao/ifttt-notify) [![Go Report Card](https://goreportcard.com/badge/github.com/seankhliao/ifttt-notify)](https://goreportcard.com/report/github.com/seankhliao/ifttt-notify)

# ifttt-notify
simple, flexible command line tool to trigger ifttt maker events

it does something similar to
```sh
curl "https://maker.ifttt.com/trigger/$(env IFTTT_EVENT)/with/key/$(IFTTT_KEY)" \
-H "Content-Type: application/json" \
-d '{"value1": "'"'$1"'", "value2": "'"$2"'", "value3", "'"$3"'"}'
```

## Install
```sh
go get github.com/seankhliao/ifttt-notify
```

## Usage
```sh
export IFTTT_EVENT=event-name
export IFTTT_KEY=your-key
ifttt-notify arg1 arg2 arg3
```
or 
```sh
ifttt-notify -event event-name -key your-key arg1 arg2 arg3
```

## License
The MIT License (MIT) - see [`LICENSE`](LICENSE) for more details
