# Haystack

To enable the Haystack:

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
```

```yaml tab="File (YAML)"
tracing:
  haystack: {}
```

```bash tab="CLI"
--tracing
--tracing.haystack
```

#### `localAgentHost`

_Require, Default="127.0.0.1"_

Local Agent Host instructs reporter to send spans to haystack-agent at this address.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    localAgentHost = "127.0.0.1"
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    localAgentHost: 127.0.0.1
```

```bash tab="CLI"
--tracing
--tracing.haystack.localAgentHost="127.0.0.1"
```

#### `localAgentPort`

_Require, Default=42699_

Local Agent port instructs reporter to send spans to the haystack-agent at this port.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    localAgentPort = 42699
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    localAgentPort: 42699
```

```bash tab="CLI"
--tracing
--tracing.haystack.localAgentPort=42699
```

#### `globalTag`

_Optional, Default=empty_

Apply shared tag in a form of Key:Value to all the traces.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    globalTag = "sample:test"
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    globalTag: sample:test
```

```bash tab="CLI"
--tracing
--tracing.haystack.globalTag="sample:test"
```

#### `traceIDHeaderName`

_Optional, Default=empty_

Specifies the header name that will be used to store the trace ID.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    traceIDHeaderName = "sample"
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    traceIDHeaderName: sample
```

```bash tab="CLI"
--tracing
--tracing.haystack.traceIDHeaderName="sample"
```

#### `parentIDHeaderName`

_Optional, Default=empty_

Specifies the header name that will be used to store the span ID.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    parentIDHeaderName = "sample"
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    parentIDHeaderName: "sample"
```

```bash tab="CLI"
--tracing
--tracing.haystack.parentIDHeaderName="sample"
```

#### `spanIDHeaderName`

_Optional, Default=empty_

Apply shared tag in a form of Key:Value to all the traces.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    spanIDHeaderName = "sample:test"
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    spanIDHeaderName: "sample:test"
```

```bash tab="CLI"
--tracing
--tracing.haystack.spanIDHeaderName=sample:test
```

#### `baggagePrefixHeaderName`

_Optional, Default=empty_

Specifies the header name prefix that will be used to store baggage items in a map.

```toml tab="File (TOML)"
[tracing]
  [tracing.haystack]
    baggagePrefixHeaderName = "sample"
```

```yaml tab="File (YAML)"
tracing:
  haystack:
    baggagePrefixHeaderName: "sample"
```


```bash tab="CLI"
--tracing
--tracing.haystack.baggagePrefixHeaderName="sample"
```