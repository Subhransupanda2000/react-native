
```

import React, { useState } from 'react';
import {

  Button,
  Text,
  View,
} from 'react-native';



const App = () => {

  const [name, SetName] = useState("terenam");

  return (
    <View>

      <Button title="updatename" onPress={() => {
        SetName("awaz");

      }}
      ></Button>
      <User name={name} />


    </View>
  );
};
const User = (props) => {
  return (
    <View>

      <Text>
        {props.name}
      </Text>

    </View>
  );
}
export default App;
```
