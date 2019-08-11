import React from 'react';
import { StyleSheet, Text, View,Image,TextInput,TouchableOpacity, Dimensions} from 'react-native';
import Constants from 'expo-constants';
import { LinearGradient } from 'expo-linear-gradient';
import { Card } from 'react-native-paper';

export default class App extends React.Component {
  constructor(props){
    super(props)
    this.state={
      num0:"0",
      num1:"1",
      num2:"2",
      num3:"3",
      num4:"4",
      num5:"5",
      num6:"6",
      num7:"7",
      num8:"8",
      num9:"9",
      value:"",
      current:"",
      previous :"",
      tmp:"",
      equal:"",
      operator:""
    }


    ///clear
  }
  acPress(){
    this.setState({value:""})
    this.setState({current:""})
    this.setState({previous :""})
    this.setState({equal:""})
    this.setState({operator:""})
  }



  //number
  zeroPress(){
    this.setState({value:this.state.value+"0"})
    this.setState({current:this.state.current+"0"})
  }
  onePress(){
    this.setState({value:this.state.value+"1"})
    this.setState({current:this.state.current+"1"})
  }
  twoPress(){
    this.setState({value:this.state.value+"2"})
    this.setState({current:this.state.current+"2"})
  }
  threePress(){
    this.setState({value:this.state.value+"3"})
    this.setState({current:this.state.current+"3"})
  }
  fourPress(){
    this.setState({value:this.state.value+"4"})
    this.setState({current:this.state.current+"4"})
  }
  fivePress(){
    this.setState({value:this.state.value+"5"})
    this.setState({current:this.state.current+"5"})
  }
  sixPress(){
    this.setState({value:this.state.value+"6"})
    this.setState({current:this.state.current+"6"})
  }
  sevenPress(){
    this.setState({value:this.state.value+"7"})
    this.setState({current:this.state.current+"7"})
  }
  eightPress(){
    this.setState({value:this.state.value+"8"})
    this.setState({current:this.state.current+"8"})
  }
  ninePress(){
    this.setState({value:this.state.value+"9"})
    this.setState({current:this.state.current+"9"})
  }
  
  //op
  plusPress(){
    this.setState({operator:"+"});
    this.setState({previous :this.state.current})
    this.setState({value:""})
    this.setState({current:""})
  }
  minusPress(){
    this.setState({operator:"-"});
    this.setState({previous :this.state.current})
    this.setState({value:""})
    this.setState({current:""})
  }
  mulPress(){
    this.setState({operator:"*"});
    this.setState({previous :this.state.current})
    this.setState({value:""})
    this.setState({current:""})
  }
  divPress(){
    this.setState({operator:"/"});
    this.setState({previous :this.state.current})
    this.setState({value:""})
    this.setState({current:""})
  }
  poPress(){
    this.setState({value:this.state.value+"."})
    this.setState({current:this.state.current+"."})
  }




///////////////////////////////////////////////////

  equalPress(){
    switch (this.state.operator){
      case "+":
        if(this.state.equal == "") {
          this.setState({value:Number(this.state.previous )+Number(this.state.current)});
          this.setState({tmp:this.state.current});
          this.setState({equal:this.state.value});
        }
        else{
          this.setState({value:Number(this.state.tmp)+Number(this.state.value)});
        }
        break;
      case "-":
          if(this.state.equal == "") {
          this.setState({value:Number(this.state.previous )-Number(this.state.current)});
          this.setState({tmp:this.state.current});
          this.setState({equal:this.state.value});
        }
        else{
          this.setState({value:Number(this.state.tmp)-Number(this.state.value)});
        }
        break;
      case "*":
          if(this.state.equal == "") {
          this.setState({value:Number(this.state.previous )*Number(this.state.current)});
          this.setState({tmp:this.state.current});
          this.setState({equal:this.state.value});
        }
        else{
          this.setState({value:Number(this.state.tmp)*Number(this.state.value)});
        }
        break;
      case "/":
          if(this.state.equal == "") {
          this.setState({value:Number(this.state.previous )/Number(this.state.current)});
          this.setState({tmp:this.state.current});
          this.setState({equal:this.state.value});
        }
        else{
          this.setState({value:Number(this.state.tmp)/Number(this.state.value)});
        }
        break;
    }
  }


  render() {
    return (

      <LinearGradient
        //https://uigradients.com/#Reef
        //https://htmlcolors.com/
        //https://facebook.github.io/react-native/docs/flexbox
        //https://github.com/tamnuwat/Basic
        //https://reactnativeexample.com/
        //https://github.com/ReactNativeSchool/react-native-calculator
        //https://docs.expo.io/versions/v34.0.0/react-native/flexbox/
        //https://facebook.github.io/react-native/docs/activityindicator
        colors={['#000000', '#000000', '#000000']}
        style={styles.container}>

        <View style={{flex: 1}}>
          <View style={{flex: 1}}>
          </View>
          <View style={{flex: 1, flexDirection: 'row',justifyContent: 'center'}}>
              <View style={{flex: 1}}>
                <Text style={styles.value} >{this.state.value}</Text>
              </View>
          </View>
           <View style={{flex: 1, flexDirection: 'row',justifyContent: 'center'}}>
              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.buttonSecondary}
              onPress={()=>this.acPress()}
              >
              <Text style={styles.textSecondary}>AC</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity style={styles.buttonSecondary}>
              <Text style={styles.textSecondary}>+/-</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity style={styles.buttonSecondary}>
              <Text style={styles.textSecondary}>%</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.buttonAccent}
              onPress={()=>this.divPress()}
              >
              <Text style={styles.text}>÷</Text>
              </TouchableOpacity>
              </View>
          </View>

           <View style={{flex: 1, flexDirection: 'row',justifyContent: 'center'}}>
              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.sevenPress()}
              >
              <Text style={styles.text}>7</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.eightPress()}
              >
              <Text style={styles.text}>8</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.ninePress()}
              >
              <Text style={styles.text}>9</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.buttonAccent}
              onPress={()=>this.mulPress()}
              >
              <Text style={styles.text}>×</Text>
              </TouchableOpacity>
              </View>
          </View>

           <View style={{flex: 1, flexDirection: 'row',justifyContent: 'center'}}>
              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.fourPress()}
              >
              <Text style={styles.text}>4</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.fivePress()}
              >
              <Text style={styles.text}>5</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.sixPress()}
              >
              <Text style={styles.text}>6</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.buttonAccent}
              onPress={()=>this.minusPress()}
              >
              <Text style={styles.text}>-</Text>
              </TouchableOpacity>
              </View>
          </View>

          <View style={{flex: 1, flexDirection: 'row',justifyContent: 'center'}}>
              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.onePress()}
              >
              <Text style={styles.text}>1</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity
              style={styles.button}
              onPress={()=>this.twoPress()}
              >
              <Text style={styles.text}>2</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.threePress()}
              >
              <Text style={styles.text}>3</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.buttonAccent}
              onPress={()=>this.plusPress()}
              >
              <Text style={styles.text}>+</Text>
              </TouchableOpacity>
              </View>
          </View>

          <View style={{flex: 1, flexDirection: 'row',justifyContent: 'center'}}>
              <View style={{flex: 2}}>
              <TouchableOpacity 
              style={styles.buttonDouble}
              onPress={()=>this.zeroPress()}
              >
              <Text style={styles.text}>0</Text>
              </TouchableOpacity>
              </View>

              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.button}
              onPress={()=>this.poPress()}
              >
              <Text style={styles.text}>.</Text>
              </TouchableOpacity>
              </View>


              <View style={{flex: 1}}>
              <TouchableOpacity 
              style={styles.buttonAccent}
              onPress={()=>this.equalPress()}
              >
              <Text style={styles.text}>=</Text>
              </TouchableOpacity>
              </View>
          </View> 
        
        </View>
      </LinearGradient>
    );
  }
}


const screen = Dimensions.get("window");
const buttonWidth = screen.width / 4;

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: "#202020",
    justifyContent: "flex-end"
  },
  value: {
    color: "#ffffff",
    fontSize: 70,
    textAlign: "right",
    marginRight: 25,
    marginBottom: 10
  },
  text: {
    color: "#fff",
    fontSize: 32
  },
  textSecondary: {
    color: "#060606",
    fontSize: 29
  },
  button: {
    backgroundColor: "#333333",
    flex: 1,
    height: Math.floor(buttonWidth - 10),
    alignItems: "center",
    justifyContent: "center",
    borderRadius: Math.floor(buttonWidth),
    margin: 7,
  },
  buttonDouble: {
    backgroundColor: "#333333",
    flex: 2,
    height: Math.floor(buttonWidth - 10),
    alignItems: "flex-start",
    justifyContent: "center",
    borderRadius: Math.floor(buttonWidth),
    paddingLeft: 40,
    margin:7
  },
  buttonSecondary: {
    backgroundColor: "#a6a6a6", // สีเทา
    flex: 1,
    height: Math.floor(buttonWidth - 10),
    alignItems: "center",
    justifyContent: "center",
    borderRadius: Math.floor(buttonWidth),
    margin: 7
  },
  buttonAccent: {
    backgroundColor: "#f09a36", // สีส้ม
    flex: 1,
    height: Math.floor(buttonWidth - 10),
    alignItems: "center",
    justifyContent: "center",
    borderRadius: Math.floor(buttonWidth),
    margin: 7
  }
})
