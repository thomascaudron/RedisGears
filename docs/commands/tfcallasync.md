--
syntax: |
    TFCALLASYNC <library name>.<function name> <number of keys> [<key1> ... <keyn>] [<arg1> ... <argn>]
--

Invoke an async function (coroutine).

## Required arguments

<details open>
<summary><code>library name</code></summary>

The name of the library that contains the function.
</details>

<details open>
<summary><code>function name</code></summary>

The function name to run.
</details>

<details open>
<summary><code>number of keys</code></summary>

The number keys that will follow.
</details>

<details open>
<summary><code>keys</code></summary>

The keys that will be touched by the function.
</details>

<details open>
<summary><code>arguments</code></summary>

The arguments passed to the function.
</details>

## Return

`TFCALLASYNC` returns either

* The return value of the function.
* [Error reply](/docs/reference/protocol-spec/#resp-errors) when the function execution failed.

## Examples

{{< highlight bash >}}
TFCALLASYNC lib.hello 0
"Hello World"
{{</ highlight>}}

## See also

## Related topics