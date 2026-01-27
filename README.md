## nucular-kindle

This is an updated example of a Kindle app made with a Nucular, a Golang framework. This works using a modified version of Shiny ([kindle-shiny](https://github.com/efskap/shiny-kindle)). Everything in this repo is derived from efskap's work - big shoutout!

## Development

You need Golang installed.

1. Clone the repository.
   ```
   git clone https://github.com/phthallo/nucular-kindle
   ```
2. Install project dependencies.
   ```
   go get
   ```
3. Make your project! Check out [nucular's](https://github.com/aarzilli/nucular) docs.
4. Test it 
   ```
   go run .
   ```
5. Build it for your device and run it with `chmod +x binarynamehere && ./binarynamehere` or double clicking it.
   ```
   go build . -o nameforyourbinaryhere
   ```
6. Build it for the Kindle. No toolchain required!
   ```
   GOARCH=arm GOARM=5 go build -o nameforyourbinaryhere_kindle
   ```