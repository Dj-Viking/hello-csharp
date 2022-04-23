# MacOS

- On my Catalina machine I had to install the dotnet binary. used the pkg file.
- however the binary itself was not placed in my $PATH so I had to manually add that myself
- when i searched within my '/' directory of my computer with command
```sh
find / -name dotnet
```
- I found the binary to be in the /usr/local/share/dotnet
- So I had to include this in my path AFTER the installation process
```sh
export PATH="$PATH:/usr/local/share/dotnet:<all the other paths to my binaries concatenated here>"
```

# Run
```sh
dotnet run

#should print "Hello, World!" to the console when in the working directory of the program.cs file
```