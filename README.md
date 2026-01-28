## nucular-kindle

This is an updated example of a Kindle app made with a Nucular, a Golang framework. This works using a modified version of Shiny ([shiny-kindle](https://github.com/efskap/shiny-kindle)). Everything in this repo is derived from efskap's work - big shoutout!

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

## Running on the Kindle

1. Jailbreak your Kindle according to the recommended jailbreak on [kindlemodding](https://kindlemodding.org/kindle-models.html)
2. Install [kterm](https://www.fabiszewski.net/kindle-terminal/). 
3. Plug in your Kindle and transfer the Kindle binary over.
4. Launch kterm with KUAL, which should be installed if the jailbreak was fully completed.
5. Navigate to the directory you put the binary in (the default working directory when you open kterm is kterm's location in the extensions folder), make the binary executable and launch it (`chmod +x binaryname_kindle && ./binaryname-kindle`)