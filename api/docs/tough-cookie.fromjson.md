<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [tough-cookie](./tough-cookie.md) &gt; [fromJSON](./tough-cookie.fromjson.md)

## fromJSON() function

Does the reverse of [Cookie.toJSON()](./tough-cookie.cookie.tojson.md)<!-- -->.

**Signature:**

```typescript
export declare function fromJSON(str: unknown): Cookie | undefined;
```

## Parameters

<table><thead><tr><th>

Parameter


</th><th>

Type


</th><th>

Description


</th></tr></thead>
<tbody><tr><td>

str


</td><td>

unknown


</td><td>

An unparsed JSON string or a value that has already been parsed as JSON


</td></tr>
</tbody></table>
**Returns:**

[Cookie](./tough-cookie.cookie.md) \| undefined

## Remarks

Any Date properties (such as .expires, .creation, and .lastAccessed) are parsed via Date.parse, not tough-cookie's parseDate, since ISO timestamps are being handled at this layer.
