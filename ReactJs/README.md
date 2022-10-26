## React JS

ReactJs merupakan sebuah library (bukan framework).<br>
website : [reactJs](reactjs.org)

## Instalasi.
Sebelum menginstall reactJs, dalam komputer harus terinstall `node js` dan `npm`. <br>
Lalu ketikkan `npx create-react-app nama-folder` pada terminal.

## ReactJS Component
Untuk membuat komponen perlu mengimport `React` lalu export default.

### StateLess Component
```javascript
const Hello = () => {
  return <p>Hello</p>
} 
```
### StateFull Component
```javascript
class Hello extends React.Component {
    render(){
        return <p>Hello</p>
    }
}
```

## Props
Peggunaan
```javascript
const Kotak = (props) => {
    return(
        <div className="kotak">
            <p>{props.nomor}</p>
        </div>
    )
}
Kotak.defaultProps = {
    nomor:'-'
}
```
Pemanggilan
```javascript
    <div style={{display:'flex',flexDirection:'row'}}>
      <Kotak nomor='1' />
      <Kotak nomor='2' />
      <Kotak  />
    </div>
```