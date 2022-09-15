## System Info

* Code: 1.71.1 (e7f30e38c5a4efafeec8ad52861eb772a9ee4dfb)
* OS: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36 Edg/105.0.1343.33(5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36 Edg/105.0.1343.33)
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
| require(workbench.desktop.main.js)                                 | 1996     | [renderer]                | cached data: NO, node_modules took 0ms   |
| wait for window config                                             | 0        | [renderer]                | -                                        |
| init storage (global & workspace)                                  | 117      | [renderer]                | -                                        |
| init workspace service                                             | 95       | [renderer]                | -                                        |
| init settings and global state from settings sync service          | 0        | [renderer]                | -                                        |
| init keybindings, snippets & extensions from settings sync service | 0        | [renderer]                | -                                        |
| register extensions & spawn extension host                         | 7208     | [renderer]                | -                                        |
| restore viewlet                                                    | 70       | [renderer]                | workbench.view.explorer                  |
| restore panel                                                      | 0        | [renderer]                | -                                        |
| restore & resolve visible editors                                  | 101      | [renderer]                | 1: workbench.editors.gettingStartedInput |
| overall workbench load                                             | 1240     | [renderer]                | -                                        |
| workbench ready                                                    | 0        | [main->renderer]          | -                                        |
| renderer ready                                                     | 3915     | [renderer]                | -                                        |
| shared process connection ready                                    | 0        | [renderer->sharedprocess] | -                                        |
| extensions registered                                              | 0        | [renderer]                | -                                        |

## Extension Activation Stats

| Extension                         | Eager | Load Code | Call Activate | Finish Activate | Event                             | By                                |
| --------------------------------- | ----- | --------- | ------------- | --------------- | --------------------------------- | --------------------------------- |
| vscode.git-base                   | true  | 3         | 1             | 0               | *                                 | vscode.git-base                   |
| vscode.github-authentication      | true  | 14        | 161           | 0               | *                                 | GitHub.vscode-pull-request-github |
| vscode.ipynb                      | true  | 14        | 3             | 0               | *                                 | vscode.ipynb                      |
| GitHub.codespaces                 | true  | 639       | 125           | 1318            | *                                 | GitHub.codespaces                 |
| GitHub.vscode-pull-request-github | true  | 96        | 0             | 843             | *                                 | GitHub.vscode-pull-request-github |
| vscode.emmet                      | false | 11        | 154           | 0               | onStartupFinished                 | vscode.emmet                      |
| vscode.extension-editing          | false | 1         | 1             | 0               | onLanguage:markdown               | vscode.extension-editing          |
| vscode.markdown-language-features | false | 33        | 7             | 199             | onLanguage:markdown               | vscode.markdown-language-features |
| vscode.markdown-math              | false | 0         | 0             | 0               | api                               | vscode.markdown-language-features |
| vscode.merge-conflict             | false | 5         | 5             | 0               | onStartupFinished                 | vscode.merge-conflict             |
| vscode.microsoft-authentication   | false | 18        | 3             | 1423            | onAuthenticationRequest:microsoft | vscode.microsoft-authentication   |
| ms-vscode.anycode                 | false | 80        | 8             | 0               | onStartupFinished                 | ms-vscode.anycode                 |

## Raw Perf Marks: renderer

```
Name	Timestamp	Delta	Total
code/timeOrigin	1663261628654	0	0
code/didStartRenderer	1663261629762	1108	1108
code/willShowPartsSplash	1663261629773	11	1119
code/didShowPartsSplash	1663261629781	8	1127
code/willLoadWorkbenchMain	1663261630049	268	1395
code/didLoadWorkbenchMain	1663261632045	1996	3391
code/willOpenDatabase/vscode-web-db	1663261632063	18	3409
code/didOpenDatabase/vscode-web-db	1663261632308	245	3654
code/registerFilesystem/vscode-log	1663261632308	0	3654
code/registerFilesystem/vscode-userdata	1663261632310	2	3656
code/registerFilesystem/file	1663261632310	0	3656
code/registerFilesystem/tmp	1663261632310	0	3656
code/willInitWorkspaceService	1663261632315	5	3661
code/willInitStorage	1663261632316	1	3662
code/willOpenDatabase/vscode-web-state-db-global	1663261632316	0	3662
code/willOpenDatabase/vscode-web-state-db--2ad0bbb	1663261632317	1	3663
code/didOpenDatabase/vscode-web-state-db-global	1663261632343	26	3689
code/didOpenDatabase/vscode-web-state-db--2ad0bbb	1663261632343	0	3689
code/willInitUserConfiguration	1663261632374	31	3720
code/didInitUserConfiguration	1663261632409	35	3755
code/willInitWorkspaceConfiguration	1663261632409	0	3755
code/didInitWorkspaceConfiguration	1663261632410	1	3756
code/didInitWorkspaceService	1663261632410	0	3756
code/didInitStorage	1663261632433	23	3779
code/willStartWorkbench	1663261632437	4	3783
code/registerFilesystem/http	1663261632464	27	3810
code/registerFilesystem/https	1663261632464	0	3810
code/LifecyclePhase/Ready	1663261632549	85	3895
code/registerFilesystem/trustedDomains	1663261632586	37	3932
code/registerFilesystem/vscode-local-history	1663261632596	10	3942
code/willRestoreEditors	1663261633573	977	4919
code/willRestoreViewlet	1663261633577	4	4923
code/didRestoreViewlet	1663261633647	70	4993
code/willLoadExtensions	1663261633672	25	5018
code/didRestoreEditors	1663261633674	2	5020
code/LifecyclePhase/Restored	1663261633677	3	5023
code/didStartWorkbench	1663261633677	0	5023
code/didRemovePartsSplash	1663261633677	0	5023
code/registerFilesystem/vscode-debug-memory	1663261633682	5	5028
code/willResumeEditSessionFromIdentifier	1663261633715	33	5061
code/didResumeEditSessionFromIdentifier	1663261633715	0	5061
code/registerFilesystem/vscode-edit-sessions	1663261633719	4	5065
code/LifecyclePhase/Eventually	1663261636178	2459	7524
code/willHandleExtensionPoints	1663261639796	3618	11142
code/didHandleExtensionPoints	1663261640858	1062	12204
code/didLoadExtensions	1663261640880	22	12226
```