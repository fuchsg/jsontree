# jsontree
A JSON tree explorer for the command line based on Python Textual

![image](https://user-images.githubusercontent.com/13031661/222457156-3c044249-a566-44fb-981a-bc211f70dd9b.png)

While exploring possibilities to move a couple of existing TUI applications based on Whiptail and also looking for a more modern look and feel I came accross the great [Textual](https://github.com/Textualize/textual) project. To familiarize myself with the concepts of that framework I took the liberty to grab one of the examples ("Tree widget") and created this little script out of it.

To us it just download it and run it like:

```
jsontree <filename>
```

Via process substitution it is also possible to use ephimeral data like:

```
jsontree <(docker inspect <dockerid>)
```
or
```
jsontree <(gcloud compute instances describe <instance> --format=json)
```
or, if you are daring (the file is huge, so it takes a while to load)
```
jsontree <(curl -sL https://github.com/fuchsg/geojson/raw/main/worldCountries-hires-10m.geojson)
```
