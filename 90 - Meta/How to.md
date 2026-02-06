# How to use this vault

This vault exists so I can capture ideas, learn properly, track project work; without everything becoming a giant unorganized mess. Like all things this solution isn't perfect, If you find this method slowing you down I encourage you to curate your very own customized experience; Since there will never be a one-size-fits-all solution when it comes to hyper-personal things like learning.

**IMPORTANT**
Git doesn't allow me to push empty folders, and adding a hidden `.gitkeep` into folders you will probably never need is redundant (Areas specific to my use-case). So I've only added them to the most basic folders like *you could need to get started*.

> [!ToDo] First thing to do once you've cloned the Template
> Create folders inside `Areas` about things you want to study/learn using this vault. Similarly create a folder with the same name inside `Resources`. [[#^26bb2f|Below I will attach the tree output of my vault to give you an idea of how to shape the vault]].

*If You're unsure where something goes, put it in `00 - Inbox/` and sort it later.*

> [!FAQ] The rule you should try to follow  
> Keep active folders small. When something stops being active, move it to `40 - Archive/` instead of letting it rot in place.

## The folders (brief overview)

`10 - Projects/` is for things You're building. If it has an outcome (ship a tool, finish an app, implement a feature set), it lives here. A project folder is allowed to be messy while You're working, because it’s a workspace. [[#What goes in a Project (10 - Projects)|More on how to work inside the Projects folder & Template]].

`20 - Areas/` is for tracks you're maintaining over time (no finish line). This is where you track what you're focusing on right now, what “good” looks like, and what you should revisit. It’s not where the actual deep notes live. [[#What goes in an Area (`20 - Areas`)|More on how to manage an Area]].

`30 - Resources/` will be the knowledge base: notes in your words, written so future you can get up to speed quickly. This is where “what I learned” lives. For rough, draft like notes which are not yet polished, use a `(raw)` suffix at the end to mark it as so. `Resources/rust/ownership/ownership_model(raw).md`. [[#What goes in Resources (30 - Resources)|More on Resources and how to work inside the folders]].

`35 - Devlog/` is for public-facing writing (==You may rename the folder as you like==). These are refined writeups that are meant to be shipped to my portfolio site. Things I understand well enough to confidently write about publically, giving an in depth technical understanding of said topic.
*If you don't plan on doing any blog writing or technical write-ups*, having a space where your best and only best notes live, is still a plus. You can use this to know how far deep your understanding is with a particular Area and continue learning until you have a huge set of that Area under this space. [[#What goes in Devlog (35 - Devlog)|More on Devlog]].

`40 - Archive/` is for inactive stuff. This keeps the active folders clean. If You're done with a project or something you haven't touched in weeks, move it here (inside the respective nested folder). If you plan to work on something again that was archived, move it back out. [[#What Archive is (40 - Archive)|More on Archives]].

`90 - Meta/` is the vault’s “operating manual”: [[#Templates (presets for some of the top level folders)|Templates]], [[#MOCs (Maps of Content)|MOCs]], and rules for how to run this workspace.

---
## What goes in a Project (`10 - Projects`)

When you get an idea and want to build it, create a folder under the  `10 - Projects/` folder and copy the Project Folder template into it.

Start with `00 - scope` first. If you can’t explain the MVP and what “done” means, you're not ready to plan tasks yet. So, the flow would be:

- `00 - scope` the idea in one paragraph, what problem it solves, MVP criteria.
- `01 - specs` features, constraints, platforms, acceptance criteria.
- `02 - architecture` for deciding how it should work. data model, API sketches, decisions, trade offs etc.
- `03 - tasks` planned tasks for that project to progress, blockers which stopped progression previously, links to sources you plan to use to help with clearing these tasks.
- *OPTIONAL* `04 - links`: For me this will contain links to published content about projects after I've shipped something worth writing about (or when I’ve drafted a post in Devlog). For you this could be sources relevant to that project, If contributing to OSS this could be links to that project repo, wiki etc.

## What goes in an Area (`20 - Areas`)

An Area is a “maintenance lane.” It’s where you track how your learning is going, what is yet to be learned and things you plan to revisit and solidify in the near future. you may use it like this:

- `00 - roadmap` a very detailed roadmap, tailored to your needs, your goals and where you want to go with this Area. You may use an LLM to generate if you feel like generic road-maps are cutting it for you (properly defined topics, tasks, something you can follow and actually grow with), go back and forth reiterating unless you're satisfied with the resulting path defined for *this* area and *it's* goals.
- `01 - now` will be your short-term focus (keep it tight. if it becomes a wishlist, it stops being useful).
- `02 - review_queue` is a list of links to the few notes you know you'll forget unless revisited. Things you want to polish up on.

If you stop maintaining an area for a while, move the whole Area folder to `40 - Archive/Areas/`.

> [!BUG] How to actually get a good roadmap to base things off of  
> Make sure you cross-check your "resulting" roadmap multiple times with multiple thinking and reasoning models. Make sure it's up to date, Make sure it actually makes you build stuff and doesn't send you off into tutorial hell.

## What goes in Resources (30 - Resources)

Resources is “learned knowledge” written so that it’s easy to revisit. If it’s unrefined, still put it here, but name it in a way that doesn’t lie to you; like adding a `(raw)` suffix.

A good Resources note usually answers:  
- What question was I trying to answer
- what’s the rule/idea in my words
- what’s a minimal example
- and what’s the one gotcha that *will* bite me later.

This folder is allowed to grow and be messy, Don't be a perfectionist. If you are one, don't follow this template and go build a better workflow because this isn't and won't ever be perfect.

## What goes in Devlog (35 - Devlog)

Devlog is the “shippable writing” lane. If I can explain the topic cleanly (or if did something worth documenting), I write it here. These notes too can be drafts until the final version is born after numerous iterations. You may use tags like #draft and #final to help track such things.

If your knowledge is half-baked on a topic, keep it in `Resources/` and link it from an Area’s `review_queue` if you want to revisit it.

## What Archive is (40 - Archive)

Archive is not a trash can. It’s a parking lot for inactive things from Projects, Areas, Resources, and Devlog. That’s the whole point of the system: active stays visible; inactive gets out of the way.​

I use Archive when:

- A project is done or abandoned.
- An area is paused, I haven't made much progress in a while and don't plan to.
- A set of notes is no longer relevant to what I'm doing right now.
- A blog draft is dead (but I don’t want to delete it).

## Templates (presets for some of the top level folders)

Templates live in `90 - Meta/Templates/`. If You're starting a new Project or planning to start learning/working on a new Area; copy the respective folder out and rename it.
```
utkarsh@arch~/D/v/n/9/Templates $ tree
.
├── Area Folder
│   ├── 00 - roadmap.md
│   ├── 01 - now.md
│   └── 02 - review_queue.md
└── Project Folder
    ├── 00 - scope.md
    ├── 01 - specs.md
    ├── 02 - architecture.md
    ├── 03 - tasks.md
    └── 04 - links.md

4 directories, 8 files
```

## MOCs (Maps of Content)

==PENDING!! Under Development==

MOCs live in `90 - Meta/MOCs/`. An MOC is just a curated “entry point” note for a topic: it links to the best Resources notes, active Areas, relevant Projects, and any Devlog posts about a specific topic/Area.

==(WIP)== A template will be included showcasing how one would implement filtering which will locate files with tags if *any one* of the conditions are met. Make sure to mark your files with an appropriate tag like so #help

> [!Example] How to actually benefit from MOCs  
> Keeping MOCs inside Area or Resources folder is redundant and breaks the flow and purpose of those folders. Whereas Meta is built for navigating the Vault, so *use MOCs to create detailed Map of Contents for your Areas and simply Bookmark them*.
> 
> I've bookmarked this `How to` note so you can easily access it under the bookmarks tab.

---
## How this will work: with various examples

When You're studying and want to take notes: you write in `30 - Resources/`.
When You're building something: you work in `10 - Projects/`.
When you want to keep your learning on track: update `20 - Areas/<Area>/01 - now` and add links to `02 - review_queue`.
When You're ready to publish a write-up: write in `35 - Devlog/`.
When something becomes inactive: move it to `40 - Archive/`.

---
## Git (keep it clean)

One commit should represent *one kind of work*. If I studied and also rewrote a devlog post, those should usually be separate commits. The goal is to make history readable later, not to "save clicks"

---

# Structure to base your personal Workspace off of: ^26bb2f

```
utkarsh@arch~/D/v/notebook $ tree --gitignore
.
├── 00 - Inbox
├── 10 - Projects
│   ├── Production     # For professional project tracking
│   └── Side Projects  # For more casual, personal projects/internal tools
├── 20 - Areas         # Your areas-of-interest go here
│   ├── DSA
│   ├── Rust
│   └── Web
├── 30 - Resources     # Mirrored, same as Areas/
│   ├── DSA
│   ├── Rust
│   └── Web
├── 35 - Devlog      # You can customize your detailed writeup space
│   ├── blogs
│   ├── notes
│   └── pages
├── 40 - Archive     # Archive inactive projects, areas, resources
│   ├── Areas          Mirror of root level folders (keep it nested)
│   ├── Devlog
│   ├── Projects
│   └── Resources
├── 90 - Meta          # Navigation & Help for the Workspace.
│   ├── How to.md
│   ├── MOCs
│   └── Templates      # Templates for Area/ and Project/ folders.
│       ├── Area Folder
│       │   ├── 00 - roadmap.md
│       │   ├── 01 - now.md
│       │   └── 02 - review_queue.md
│       └── Project Folder
│           ├── 00 - scope.md
│           ├── 01 - specs.md
│           ├── 02 - architecture.md
│           ├── 03 - tasks.md
│           └── 04 - links.md
├── _assets
│   ├── diagrams       # Excalidraw drawings go here by default
│   └── images         # Images are auto sorted into nested folders
│       └── README
│           ├── IMG-20260206163250296.png
│           ├── IMG-20260206164013920.png
│           └── IMG-20260206165129843.png
└── README.md
```
