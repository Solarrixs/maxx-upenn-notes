> [!columns|no-t] Note Statistics
> > [!info|ttl-c no-i] Note Types
> > - `$=dv.el("b", dv.pages().length)` total notes.
> > - `$=dv.el("b", dv.pages('"000 System Files/Journal"').length)` journal entries.
> > - `$=dv.el("b", dv.pages('"300 Areas/Personal Writing"').length)` personal blogs.
>
> > [!info|ttl-c no-i] Reading Notes
> > - `$=dv.el("b", dv.pages('"200 Resources/Articles & Books/Articles"').length)` articles processed.
> > - `$=dv.el("b", dv.pages('"200 Resources/Articles & Books/Books"').length)` books processed.
> > - `$=dv.el("b", dv.pages('"300 Areas/Academia"').length)` literature reviews processed.

> [!columns|ttl-c no-t] MOCs
>
> > [!info|c-pink no-i] Active MOCs
> > ```dataview
> > LIST
> > WHERE type = "MOC" AND file.name != "000 MOC"
> > ```
>
> > [!info|c-pink no-i] MOC Trackers
> > ```dataview
> > LIST
> > WHERE type = "MOC/Tracker"
> > ```

> [!column|c-purple bg-purple ttl-c dataview 2 no-i] Inactive MOCs
> ```dataview
> LIST
> WHERE type = "MOC/Inactive"
> SORT type asc
> ```

> [!column|c-yellow bg-yellow ttl-c dataview 1 no-i] Tasks
> ```dataview
> TASK
> FROM "000 System Files/Journal"
> WHERE !completed AND file.name !=this.file.name AND meta(section).subpath = "Workbench"
> ```