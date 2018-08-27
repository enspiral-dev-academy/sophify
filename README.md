# Sophify
A command line tool for assembling education curricula

soph: from the greek Sophia meaning wisdom and ify: "to make or cause to become"

Sophify is a tool to help educators assemble small, independent pieces of curriculum into a course just as developers build apps by assembling many libraries. 

**This app is under early development and not ready for use.**

## Terminology

- segment: an individual piece of curriculum. Each segment is a standalone node module 
- course: a programme of learning built on top of multiple segments

## Intended usage

```
sophify init #create a sophify.json file and setup initial folder structures
sophify build #build all the curriculum
sophify add [segment-name] #add a new segment to the course (wraps npm install)
sophify remove [segment-name] #remove a segment from the course (wraps npm uninstall)
```

## Key tech

- [gitbook](https://github.com/GitbookIO/gitbook) for managing student and teaching guides
- [revealjs](https://github.com/hakimel/reveal.js) for slides

## Folder structure
```
./segments/ #a segments
./student-guide/ #gitbook for student facing materials
./teaching-guide/ #gitbook for teacher facing materials
./slides/ #slide decks for the segments


```

## sophify.json

### for a segment
```
{
  "sophify-type": "segment"
}
```

### for a course
```
{
  "sophy-type": "course"
}
```
