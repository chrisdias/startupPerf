## System Info

* Code: 1.71.1 (e7f30e38c5a4efafeec8ad52861eb772a9ee4dfb)
* OS: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36(5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36)
* VM(likelihood): 0%
* Initial Startup: false
* Has 0 other windows
* Screen Reader Active: false
* Empty Workspace: false

## Performance Marks

| What                                                               | Duration | Process                   | Info                                     |
| ------------------------------------------------------------------ | -------- | ------------------------- | ---------------------------------------- |
| start => app.isReady                                               | -        | [main]                    | initial startup: false                   |
| nls:start => nls:end                                               | -        | [main]                    | initial startup: false                   |
| require(main.bundle.js)                                            | -        | [main]                    | initial startup: false                   |
| start crash reporter                                               | -        | [main]                    | initial startup: false                   |
| serve main IPC handle                                              | -        | [main]                    | initial startup: false                   |
| create window                                                      | -        | [main]                    | initial startup: false,                  |
| app.isReady => window.loadUrl()                                    | -        | [main]                    | initial startup: false                   |
| window.loadUrl() => begin to require(workbench.desktop.main.js)    | 0        | [main->renderer]          | NewWindow                                |
| require(workbench.desktop.main.js)                                 | 1306     | [renderer]                | cached data: NO, node_modules took 0ms   |
| wait for window config                                             | 0        | [renderer]                | -                                        |
| init storage (global & workspace)                                  | 1475     | [renderer]                | -                                        |
| init workspace service                                             | 717      | [renderer]                | -                                        |
| init settings and global state from settings sync service          | 0        | [renderer]                | -                                        |
| init keybindings, snippets & extensions from settings sync service | 0        | [renderer]                | -                                        |
| register extensions & spawn extension host                         | 1093     | [renderer]                | -                                        |
| restore viewlet                                                    | 52       | [renderer]                | workbench.view.explorer                  |
| restore panel                                                      | 0        | [renderer]                | -                                        |
| restore & resolve visible editors                                  | 101      | [renderer]                | 1: workbench.editors.gettingStartedInput |
| overall workbench load                                             | 632      | [renderer]                | -                                        |
| workbench ready                                                    | 0        | [main->renderer]          | -                                        |
| renderer ready                                                     | 3719     | [renderer]                | -                                        |
| shared process connection ready                                    | 0        | [renderer->sharedprocess] | -                                        |
| extensions registered                                              | 0        | [renderer]                | -                                        |

## Extension Activation Stats

| Extension                         | Eager | Load Code | Call Activate | Finish Activate | Event                             | By                                |
| --------------------------------- | ----- | --------- | ------------- | --------------- | --------------------------------- | --------------------------------- |
| vscode.git-base                   | true  | 3         | 0             | 0               | *                                 | vscode.git-base                   |
| vscode.ipynb                      | true  | 11        | 2             | 0               | *                                 | vscode.ipynb                      |
| vscode.emmet                      | false | 10        | 31            | 0               | onStartupFinished                 | vscode.emmet                      |
| vscode.extension-editing          | false | 2         | 0             | 0               | onLanguage:markdown               | vscode.extension-editing          |
| vscode.github-authentication      | false | 14        | 2             | 1               | onAuthenticationRequest:github    | vscode.github-authentication      |
| vscode.markdown-language-features | false | 36        | 8             | 183             | onLanguage:markdown               | vscode.markdown-language-features |
| vscode.markdown-math              | false | 1         | 0             | 0               | api                               | vscode.markdown-language-features |
| vscode.merge-conflict             | false | 2         | 7             | 0               | onStartupFinished                 | vscode.merge-conflict             |
| vscode.microsoft-authentication   | false | 20        | 2             | 213             | onAuthenticationRequest:microsoft | vscode.microsoft-authentication   |

## Raw Perf Marks: renderer

```
Name	Timestamp	Delta	Total
code/timeOrigin	1663259810937	0	0
code/didStartRenderer	1663259811138	201	201
code/willShowPartsSplash	1663259811144	6	207
code/didShowPartsSplash	1663259811213	69	276
code/willLoadWorkbenchMain	1663259811371	158	434
code/didLoadWorkbenchMain	1663259812677	1306	1740
code/willOpenDatabase/vscode-web-db	1663259812679	2	1742
code/didOpenDatabase/vscode-web-db	1663259812720	41	1783
code/registerFilesystem/vscode-log	1663259812724	4	1787
code/registerFilesystem/vscode-userdata	1663259812734	10	1797
code/registerFilesystem/file	1663259812734	0	1797
code/registerFilesystem/tmp	1663259812734	0	1797
code/willInitWorkspaceService	1663259812741	7	1804
code/willInitStorage	1663259812746	5	1809
code/willOpenDatabase/vscode-web-state-db-global	1663259812747	1	1810
code/willOpenDatabase/vscode-web-state-db--2ad0bbb	1663259812748	1	1811
code/didOpenDatabase/vscode-web-state-db-global	1663259812847	99	1910
code/didOpenDatabase/vscode-web-state-db--2ad0bbb	1663259812854	7	1917
code/willInitUserConfiguration	1663259813418	564	2481
code/didInitUserConfiguration	1663259813456	38	2519
code/willInitWorkspaceConfiguration	1663259813456	0	2519
code/didInitWorkspaceConfiguration	1663259813457	1	2520
code/didInitWorkspaceService	1663259813458	1	2521
code/didInitStorage	1663259814221	763	3284
code/willStartWorkbench	1663259814225	4	3288
code/registerFilesystem/http	1663259814247	22	3310
code/registerFilesystem/https	1663259814247	0	3310
code/LifecyclePhase/Ready	1663259814320	73	3383
code/registerFilesystem/trustedDomains	1663259814349	29	3412
code/registerFilesystem/vscode-local-history	1663259814356	7	3419
code/willRestoreEditors	1663259814754	398	3817
code/willRestoreViewlet	1663259814778	24	3841
code/didRestoreViewlet	1663259814830	52	3893
code/willLoadExtensions	1663259814852	22	3915
code/didRestoreEditors	1663259814855	3	3918
code/LifecyclePhase/Restored	1663259814856	1	3919
code/didStartWorkbench	1663259814857	1	3920
code/didRemovePartsSplash	1663259814857	0	3920
code/registerFilesystem/vscode-debug-memory	1663259814862	5	3925
code/willResumeEditSessionFromIdentifier	1663259814908	46	3971
code/didResumeEditSessionFromIdentifier	1663259814908	0	3971
code/registerFilesystem/vscode-edit-sessions	1663259814915	7	3978
code/willHandleExtensionPoints	1663259815455	540	4518
code/didHandleExtensionPoints	1663259815896	441	4959
code/didLoadExtensions	1663259815945	49	5008
```