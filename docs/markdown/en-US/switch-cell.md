## SwitchCell
`SwitchCell` component is an encapsulation of `Switch` and `Cell`.

### Install
``` javascript
import { SwitchCell } from 'vant';

Vue.use(SwitchCell);
```

### Usage

#### Basic Usage

```html
<van-cell-group>
  <van-switch-cell v-model="checked" title="Title" />
</van-cell-group>
```

```javascript
export default {
  data() {
    return {
      checked: true
    }
  }
}
```


#### Disabled
use `disabled` property to disable the component

```html
<van-cell-group>
  <van-switch-cell v-model="checked" disabled title="Title" />
</van-cell-group>
```


#### Loading
use `loading` property to keep component in loading state

```html
<van-cell-group>
  <van-switch-cell v-model="checked" loading title="Title" />
</van-cell-group>
```

### API

| Attribute | Description | Type | Default | Accepted Values |
|-----------|-----------|-----------|-------------|-------------|
| v-model | on-off state of the switch | `Boolean` | - | - |
| title | the leftside title |  `String` | `''` | - |
| loading | whether the component is in loading state |  `Boolean` | `false` | - |
| disabled | whether to disable the component |  `Boolean` | `false` | - |

### Event

| Event | Description | Arguments |
|-----------|-----------|-----------|
| change | triggered when the on-off state is changed | checked: switch is on or not |