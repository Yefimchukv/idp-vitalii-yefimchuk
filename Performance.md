# Performance

[к оглавлению](./README.md)

## Содержание

- [UI Performance](./Performance.md#ui-performance)
- [App Performance](./Performance.md#app-performance)
- [Core (language)](./Performance.md#core-language)

## <a id="ui-performance)"></a> UI Performance

## Qualified:
### 1. Understands how to build a layout with and without auto layout
    * ?
### 2. Knows what is «reusing» and what can be reused in UIKit
    * ?
### 3. Knows what issues may occur during reusing (in the context of async operations)
    * ?
### 4. Knows how to solve layout issues (ambiguous and unsatisfiable layouts)
    * ?

## Competent:
### 1. Knows what logical operations may block UI and how to avoid them (heavyweight objects creation like Formatters, data loading, …)
    * ?
### 2. Understands Auto layout cycle steps (update, layout and render steps) and corresponding UIView callbacks, how to avoid infinite layout cycle loop (not to ### trigger previous layout phase)
    * ?
### 3. Knows what factors affect collections (UITableView, UICollectionVIew) scroll performance (reuse, blended layers, rasterization, content size calculations)
    * ?
### 4. Knows how shadows can slow down UI and how to deal with them
    * ?

## - Expert:
### 1. Knows how to profile performance issues
    * ?

## <a id="app-performance)"></a> App Performance

## Qualified:
### 1. Knows concurrency basics (GCD queues, async/sync, groups)
// GROUP
GDC - Grand Central Dispatch, основной метод управления многозадачностью в iOS. 
Имеет main(всегда Serial, `критически важен для обновления UI`) и global(QOS, всегда Concurrent).
Quality of Service делится на: default, userInteractive, userInitiated, utility, background.
При работе с очередями мы можем отправлять запросы на выполнение синхронно или асинхронно. Синхронные очереди добавляют задачи в конец очереди и ожидают их выполение. В асинхронных очередях не происходит ожидание выполнения.
### 2. Knows how memory management works (ARC, reference counter)
ARC - автоматический счетчик ссылок. Удерживает в памяти ссылаемые обьекты и удаляет их в случае "высвобождения". Сильные ссылки повышают/понижают ARC, weak/unowned - нет. Unowned не должен быть nil
### 3. Knows what retain cycle is and how to avoid it
// retain cycle with nonescaping cosures
// retain cycle with delegates
Reatin cycle это ситуация, когда ARC не высвободил необхдимые обьекты. Можно избежать привязыванием обьектов слабыми ссылками, также важно помнить о weak/unowned self внутри замыкания.
### 4. Knows about potential memory problems in closures and how to avoid them (context capturing, retain cycles)
    * ?

## Competent:
### 1. Knows how to react to memory pressure (memory warnings)
    * ?
### 2. Big data uploading - problems, solutions (mostly about memory management)
    * ? 
### 3. Knows when and how to use autorelease pool
    * ?
### 4. Knows OperationQueue basics (configuration, usage, dependencies, types of operations)
    * ?

## - Expert:
### 1. Can describe pros/cons of OperationQueue and GCD usage
    * ?
### 2. Understands what are Locks, types of locks, their purpose, and usage
    * ?
### 3. Compiler optimizations (single file/whole module, size/speed). Knows, what compiler do in each mode
    * ?
### 4. Knows and keeps in mind complexity theory, Big-O notations (can explain what is complexity, good examples, and negative examples from experience)
    * ?

## <a id="core-language"></a> Core (language)

## Qualified:
### 1. Uses appropriate data structures (arrays, sets, dictionaries - purpose, differences)
    //read difference
### 2. Understands difference between value & reference types
    * ?

## Competent:
### 1. Understands what is Copy-on-write optimization
    * ?
    
## - Expert:
### 1. static vs. dynamic dispatches (how, when and why, performance)
    * ?
### 2. Knows about technics to reduce compilation time (!Measuring!, type inference, multiple targets)
    * ?
