## System Info

* Code: 1.71.1 (e7f30e38c5a4efafeec8ad52861eb772a9ee4dfb)
* OS: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.6.1 Safari/605.1.15(5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.6.1 Safari/605.1.15)
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
| require(workbench.desktop.main.js)                                 | 578      | [renderer]                | cached data: NO, node_modules took 0ms   |
| wait for window config                                             | 0        | [renderer]                | -                                        |
| init storage (global & workspace)                                  | 75       | [renderer]                | -                                        |
| init workspace service                                             | 71       | [renderer]                | -                                        |
| init settings and global state from settings sync service          | 0        | [renderer]                | -                                        |
| init keybindings, snippets & extensions from settings sync service | 0        | [renderer]                | -                                        |
| register extensions & spawn extension host                         | 1198     | [renderer]                | -                                        |
| restore viewlet                                                    | 79       | [renderer]                | workbench.view.explorer                  |
| restore panel                                                      | 0        | [renderer]                | -                                        |
| restore & resolve visible editors                                  | 84       | [renderer]                | 1: workbench.editors.gettingStartedInput |
| overall workbench load                                             | 412      | [renderer]                | -                                        |
| workbench ready                                                    | 0        | [main->renderer]          | -                                        |
| renderer ready                                                     | 1187     | [renderer]                | -                                        |
| shared process connection ready                                    | 0        | [renderer->sharedprocess] | -                                        |
| extensions registered                                              | 0        | [renderer]                | -                                        |

## Extension Activation Stats

| Extension                         | Eager | Load Code | Call Activate | Finish Activate | Event                             | By                                |
| --------------------------------- | ----- | --------- | ------------- | --------------- | --------------------------------- | --------------------------------- |
| vscode.git-base                   | true  | 1         | 1             | 0               | *                                 | vscode.git-base                   |
| vscode.ipynb                      | true  | 16        | 7             | 0               | *                                 | vscode.ipynb                      |
| GitHub.codespaces                 | true  | 82        | 6             | 134             | *                                 | GitHub.codespaces                 |
| vscode.emmet                      | false | 5         | 20            | 0               | onStartupFinished                 | vscode.emmet                      |
| vscode.extension-editing          | false | 4         | 1             | 0               | onLanguage:markdown               | vscode.extension-editing          |
| vscode.github-authentication      | false | 7         | 3             | 1               | api                               | GitHub.codespaces                 |
| vscode.markdown-language-features | false | 73        | 68            | 288             | onLanguage:markdown               | vscode.markdown-language-features |
| vscode.markdown-math              | false | 1         | 0             | 0               | api                               | vscode.markdown-language-features |
| vscode.merge-conflict             | false | 2         | 4             | 0               | onStartupFinished                 | vscode.merge-conflict             |
| vscode.microsoft-authentication   | false | 10        | 2             | 254             | onAuthenticationRequest:microsoft | vscode.microsoft-authentication   |
| ms-vscode.anycode                 | false | 56        | 5             | 1               | onStartupFinished                 | ms-vscode.anycode                 |

## Raw Perf Marks: renderer

```
Name	Timestamp	Delta	Total
code/timeOrigin	1663259798687	0	0
code/didStartRenderer	1663259798702	15	15
code/willShowPartsSplash	1663259798710	8	23
code/didShowPartsSplash	1663259798798	88	111
code/willLoadWorkbenchMain	1663259798804	6	117
code/didLoadWorkbenchMain	1663259799382	578	695
code/willOpenDatabase/vscode-web-db	1663259799384	2	697
code/registerFilesystem/vscode-log	1663259799392	8	705
code/didOpenDatabase/vscode-web-db	1663259799392	0	705
code/registerFilesystem/tmp	1663259799393	1	706
code/registerFilesystem/vscode-userdata	1663259799393	0	706
code/willInitWorkspaceService	1663259799397	4	710
code/willOpenDatabase/vscode-web-state-db--2ad0bbb	1663259799398	1	711
code/willInitStorage	1663259799398	0	711
code/willOpenDatabase/vscode-web-state-db-global	1663259799398	0	711
code/didOpenDatabase/vscode-web-state-db-global	1663259799407	9	720
code/didOpenDatabase/vscode-web-state-db--2ad0bbb	1663259799412	5	725
code/willInitUserConfiguration	1663259799465	53	778
code/willInitWorkspaceConfiguration	1663259799467	2	780
code/didInitUserConfiguration	1663259799467	0	780
code/didInitWorkspaceConfiguration	1663259799468	1	781
code/didInitWorkspaceService	1663259799468	0	781
code/didInitStorage	1663259799473	5	786
code/willStartWorkbench	1663259799477	4	790
code/registerFilesystem/https	1663259799496	19	809
code/registerFilesystem/http	1663259799496	0	809
code/LifecyclePhase/Ready	1663259799564	68	877
code/registerFilesystem/trustedDomains	1663259799587	23	900
code/registerFilesystem/vscode-local-history	1663259799598	11	911
code/willRestoreEditors	1663259799802	204	1115
code/willRestoreViewlet	1663259799806	4	1119
code/didRestoreViewlet	1663259799885	79	1198
code/didRestoreEditors	1663259799886	1	1199
code/willLoadExtensions	1663259799886	0	1199
code/LifecyclePhase/Restored	1663259799889	3	1202
code/didRemovePartsSplash	1663259799889	0	1202
code/didStartWorkbench	1663259799889	0	1202
code/registerFilesystem/vscode-debug-memory	1663259799897	8	1210
code/didResumeEditSessionFromIdentifier	1663259799946	49	1259
code/willResumeEditSessionFromIdentifier	1663259799946	0	1259
code/registerFilesystem/vscode-edit-sessions	1663259799952	6	1265
code/willHandleExtensionPoints	1663259800989	1037	2302
code/didHandleExtensionPoints	1663259801079	90	2392
code/didLoadExtensions	1663259801084	5	2397