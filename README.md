# chords-db
This is a javascript database of string instruments chords. Open, free to use, easily improved with more chords. 
Contributions are welcomed, still a lot of chords (and instruments) missing. 
Use the pull request feature of Github to add your desired chords if you want to contribute.

Take a look at the chords database of an instrument to understand the schema used to register new chords.
For example, let's take a look at the Csus2 chords of guitar. We can see this information in the C/sus2.js file:

```
export default {
  key: 'D',
  suffix: 'sus2',
  positions: [{
    frets: '0320xx',
    fingers: '031000'
  },
  {
    frets: '55775x',
    fingers: '114310',
    barres: 5,
    capo: true
  }]
}

```

Each *position* define a new chord variation of the Dsus2 chord.
We must define the *frets* needed to obtain the chord in the respective strings.
We can define too the *fingers* information for easy reading of the chord.
If the chord need to barre some string, we will define if in the *barre* field. If
you want the barre be represented with capo, you can define the "capo" property too.

This information will render this two chords using an SVG renderer I'm coding here.

[react-chords](https://tombatossals.github.io/react-chords)

You can take a look of the current state of the database in this site:

[chord-collection](https://chord-collection.com)

