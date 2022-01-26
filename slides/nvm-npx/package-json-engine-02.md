package.json "engines" value

can lead to warnings during `npm install`

<small>
  even if that version is used only for development and build purposes
</small>

```bash
npm WARN EBADENGINE Unsupported engine {
npm WARN EBADENGINE   package: 'package_name@0.0.1',
npm WARN EBADENGINE   required: { node: '>=10.0.0 <15' },
npm WARN EBADENGINE   current: { node: 'v16.13.1', npm: '8.1.2' }
npm WARN EBADENGINE }
```

<aside class="notes">
</aside>
