# react-native-ripple-button-reanimated

### **Description**: 
This is a button component with ripple effect. It works with both android and ios.

### **Requirements**:
1. react-native-reanimated: >= 2.0.0-rc.0
2. react-native-gesture-handler

### **Installation**: 

yarn: 
```
yarn add react-native-ripple-button-reanimated
```

npm:

```
npm install react-native-ripple-button-reanimated
```

### **Usage**:
```react
...

import { RippleButton } from 'react-native-ripple-button-reanimated';
import { View, Text } from 'react-native';

...

function MyRippleComponent() {
  return (
    <RippleButton
      onPress={() => console.log('Some magic here')}
      color="#fff" // background color of button.
      rippleColor="#000" // ripple effect with your favorite color.
      rippleOpacity={0.3}
      rippleScale={1} // maximize scale of ripple effect.
      duration={250} // time the ripple effect will be spread out to the edge of button.
      borderRadius={9999} // border radius of ripple effect
    >
      <View style={{ 
        width: 150, 
        height: 150, 
        borderRadius: 75 
        justifyContent: 'center',
        alignItems: 'center',
      }}>
        <Text> 
          Click me
        </Text>
      </View>
    </RippleButton>
  );
}

...
export default MyRippleComponent;
```
