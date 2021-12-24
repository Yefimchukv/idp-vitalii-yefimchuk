# Perfomance

[к оглавлению](./README.md)

## Содержание

- [UI Perfomance](./Perfomance.md#ui-perfomance)
- [App Perfomance](./Perfomance.md#app-perfomance)
- [Core (language)](./Perfomance.md#core-language)

## <a id="ui-perfomance)"></a> UI Perfomance

- Qualified:
1. Understands how to build a layout with and without auto layout
2. Knows what is «reusing» and what can be reused in UIKit
3. Knows what issues may occur during reusing (in the context of async operations)
4. Knows how to solve layout issues (ambiguous and unsatisfiable layouts)

- Competent:
1. Knows what logical operations may block UI and how to avoid them (heavyweight objects creation like Formatters, data loading, …)
2. Understands Auto layout cycle steps (update, layout and render steps) and corresponding UIView callbacks, how to avoid infinite layout cycle loop (not to trigger previous layout phase)
3. Knows what factors affect collections (UITableView, UICollectionVIew) scroll performance (reuse, blended layers, rasterization, content size calculations)
4. Knows how shadows can slow down UI and how to deal with them

- Expert:
1. Knows how to profile performance issues

## <a id="app-perfomance)"></a> App Perfomance

- Qualified:
1. Knows concurrency basics (GCD queues, async/sync, groups)
2. Knows how memory management works (ARC, reference counter)
3. Knows what retain cycle is and how to avoid it
4. Knows about potential memory problems in closures and how to avoid them (context capturing, retain cycles)

- Competent:
1. Knows how to react to memory pressure (memory warnings)
2. Big data uploading - problems, solutions (mostly about memory management) 
3. Knows when and how to use autorelease pool
4. Knows OperationQueue basics (configuration, usage, dependencies, types of operations)

- Expert:
1. Can describe pros/cons of OperationQueue and GCD usage
2. Understands what are Locks, types of locks, their purpose, and usage
3. Compiler optimizations (single file/whole module, size/speed). Knows, what compiler do in each mode
4. Knows and keeps in mind complexity theory, Big-O notations (can explain what is complexity, good examples, and negative examples from experience)

## <a id="core-language"></a> Core (language)

- Qualified:
1. Uses appropriate data structures (arrays, sets, dictionaries - purpose, differences)
2. Understands difference between value & reference types

- Competent:
1. Understands what is Copy-on-write optimization
2. Expert:

- Expert
1. static vs. dynamic dispatches (how, when and why, performance)
2. Knows about technics to reduce compilation time (!Measuring!, type inference, multiple targets)
