<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FurnitureCatalog.jsx</title>
</head>

<body>
  <h1>FurnitureCatalog.jsx</h1>
  <p>
  <pre>
     <code>
import { useState, useEffect } from 'react'
import { useStore } from './store.js'

const FurnitureCatalog = () => {
const room = useStore((state) => state.room)
const setRoom = useStore((state) => state.setRoom)
const cameraView = useStore((s) => s.cameraView)
const setCameraView = useStore((s) => s.setCameraView)

const addFurniture = useStore((state) => state.addFurniture)
const furniture = useStore((state) => state.furniture)

const [localRoom, setLocalRoom] = useState(room)

useEffect(() => { setLocalRoom(room) }, [room])

const handleChange = (field, value) => {
let val = value
if (field !== 'displayMode' && typeof value === 'string' && !isNaN(Number(value))) {
val = parseFloat(value)
}
const next = { ...localRoom, [field]: val }
setLocalRoom(next)
setRoom(next)
}

const getBtnStyle = (viewName) => ({
flex: 1, padding: '8px',
background: cameraView === viewName ? '#4db6ac' : '#1a1a2e',
color: cameraView === viewName ? '#fff' : '#ccc',
border: `1px solid ${cameraView === viewName ? '#4db6ac' : '#444'}`,
borderRadius: '4px', cursor: 'pointer', fontSize: '12px', transition: 'all 0.2s'
})

const furnBtnStyle = {
padding: '8px', background: '#333', color: '#fff', border: '1px solid #555',
borderRadius: '4px', cursor: 'pointer', flex: 1, fontSize: '12px'
}

return (
&lt;div className="furniture-catalog"&gt;
  &lt;h3&gt;🛋 Конструктор мебели&lt;/h3&gt;

  {/* Камера */}
  &lt;div style={{ marginBottom: '20px' }}&gt;
    &lt;label style={{ display: 'block' , marginBottom: '8px' , fontSize: '12px' , color: '#888' }}&gt;Вид камеры&lt;/label&gt;
    &lt;div style={{ display: 'flex' , gap: '8px' , marginBottom: '8px' }}&gt;
      &lt;button onClick={()=&gt; setCameraView('front')} style={getBtnStyle('front')}&gt;Спереди&lt;/button&gt;
      &lt;button onClick={()=&gt; setCameraView('top')} style={getBtnStyle('top')}&gt;Сверху&lt;/button&gt;
    &lt;/div&gt;
    &lt;div style={{ display: 'flex' , gap: '8px' , marginBottom: '8px' }}&gt;
      &lt;button onClick={()=&gt; setCameraView('left')} style={getBtnStyle('left')}&gt;Слева&lt;/button&gt;
      &lt;button onClick={()=&gt; setCameraView('right')} style={getBtnStyle('right')}&gt;Справа&lt;/button&gt;
    &lt;/div&gt;
    &lt;button onClick={()=&gt; setCameraView('free')} style={{ width: '100%', ...getBtnStyle('free') }}&gt;Свободный&lt;/button&gt;
  &lt;/div&gt;

  {/* Размеры */}
  &lt;div style={{ marginBottom: '15px' }}&gt;
    &lt;label style={{ fontSize: '13px' , color: '#ccc' }}&gt;Размеры комнаты (м)&lt;/label&gt;
    {['height', 'width', 'depth'].map(dim =&gt; (
    &lt;div key={dim} style={{ marginTop: '5px' }}&gt;
      &lt;span style={{ fontSize: '12px' , color: '#888' , textTransform: 'capitalize' }}&gt;{dim}:&lt;/span&gt;
      &lt;input type="number" step="0.1" value={localRoom[dim]} onChange={(e)=&gt; handleChange(dim, e.target.value)}
      style={{ width: '100%', padding: '5px', background: '#222', border: '1px solid #444', color: 'white' }}
      /&gt;
    &lt;/div&gt;
    ))}
  &lt;/div&gt;

  {/* --- ВОТ ЭТО МЫ ВЕРНУЛИ: Цвета --- */}
  &lt;div style={{ marginBottom: '15px' , display: 'flex' , gap: '10px' }}&gt;
    &lt;div style={{ flex: 1 }}&gt;
      &lt;label style={{ fontSize: '12px' , color: '#888' }}&gt;Стены&lt;/label&gt;
      &lt;div style={{ display: 'flex' , alignItems: 'center' , background: '#222' , padding: '4px' ,
        border: '1px solid #444' , borderRadius: '4px' }}&gt;
        &lt;input type="color" value={localRoom.wallColor || '#eeeeee' } onChange={(e)=&gt; handleChange('wallColor',
        e.target.value)}
        style={{ border: 'none', width: '25px', height: '25px', cursor: 'pointer', background: 'none' }}
        /&gt;
        &lt;span style={{ marginLeft: '8px' , fontSize: '12px' , color: '#ccc' }}&gt;{localRoom.wallColor}&lt;/span&gt;
      &lt;/div&gt;
    &lt;/div&gt;
    &lt;div style={{ flex: 1 }}&gt;
      &lt;label style={{ fontSize: '12px' , color: '#888' }}&gt;Пол&lt;/label&gt;
      &lt;div style={{ display: 'flex' , alignItems: 'center' , background: '#222' , padding: '4px' ,
        border: '1px solid #444' , borderRadius: '4px' }}&gt;
        &lt;input type="color" value={localRoom.floorColor || '#8d6e63' } onChange={(e)=&gt; handleChange('floorColor',
        e.target.value)}
        style={{ border: 'none', width: '25px', height: '25px', cursor: 'pointer', background: 'none' }}
        /&gt;
        &lt;span style={{ marginLeft: '8px' , fontSize: '12px' , color: '#ccc' }}&gt;{localRoom.floorColor}&lt;/span&gt;
      &lt;/div&gt;
    &lt;/div&gt;
  &lt;/div&gt;

  {/* Режимы */}
  &lt;div style={{ marginBottom: '15px' }}&gt;
    &lt;label style={{ fontSize: '13px' , color: '#ccc' }}&gt;🎨 Режим отображения&lt;/label&gt;
    &lt;div style={{ display: 'grid' , gridTemplateColumns: '1fr 1fr' , gap: '5px' , marginTop: '5px' }}&gt;
      {['textured', 'wireframe', 'transparent', 'grid'].map(mode =&gt; (
      &lt;button key={mode} onClick={()=&gt; handleChange('displayMode', mode)}
        style={{
        padding: '6px',
        background: localRoom.displayMode === mode ? '#4db6ac' : '#222',
        color: localRoom.displayMode === mode ? '#fff' : '#ccc',
        border: '1px solid #444',
        borderRadius: '4px',
        cursor: 'pointer',
        fontSize: '12px'
        }}
        &gt;
        {mode === 'textured' ? 'Текстуры' : mode === 'wireframe' ? 'Каркас' : mode === 'transparent' ? 'Прозрачный' :
        'Сетка'}
      &lt;/button&gt;
      ))}
    &lt;/div&gt;
  &lt;/div&gt;

  {/* Сетка */}
  {localRoom.displayMode === 'grid' && (
  &lt;div style={{ marginBottom: '15px' , padding: '10px' , background: '#222' , borderRadius: '6px' ,
    border: '1px dashed #444' }}&gt;
    &lt;label style={{ display: 'flex' , flexDirection: 'column' , gap: '8px' , fontSize: '13px' , color: '#ccc' }}&gt;
      &lt;div style={{ display: 'flex' , justifyContent: 'space-between' , alignItems: 'center' }}&gt;
        &lt;span&gt;Шаг сетки (мм):&lt;/span&gt;
        &lt;input type="number" min="100" max="2000" step="50" value={Math.round((localRoom.gridSpacing || 0.5) * 1000)}
          onChange={(e)=&gt; {
        let valMm = parseInt(e.target.value)
        if (isNaN(valMm)) valMm = 500
        const valM = valMm / 1000
        handleChange('gridSpacing', valM)
        }}
        style={{ width: '60px', padding: '2px 5px', fontSize: '12px', textAlign: 'right', background: '#333', border:
        '1px solid #555', color: '#fff', borderRadius: '4px' }}
        /&gt;
      &lt;/div&gt;
      &lt;input type="range" min="0.1" max="2.0" step="0.05" value={localRoom.gridSpacing || 0.5} onChange={(e)=&gt;
      handleChange('gridSpacing', parseFloat(e.target.value))}
      style={{ width: '100%', cursor: 'pointer' }}
      /&gt;
    &lt;/label&gt;
  &lt;/div&gt;
  )}

  {/* Каталог Мебели */}
  &lt;div style={{ marginTop: '20px' , paddingTop: '15px' , borderTop: '1px solid #444' }}&gt;
    &lt;div style={{ marginBottom: '10px' , fontSize: '14px' , fontWeight: 'bold' }}&gt;Добавить мебель&lt;/div&gt;
    &lt;div style={{ display: 'flex' , gap: '10px' }}&gt;
      &lt;button onClick={()=&gt; addFurniture('armchair')} style={furnBtnStyle}&gt;Кресло&lt;/button&gt;
      &lt;button onClick={()=&gt; addFurniture('table')} style={furnBtnStyle}&gt;Стол&lt;/button&gt;
      &lt;button onClick={()=&gt; addFurniture('cabinet')} style={furnBtnStyle}&gt;Шкаф&lt;/button&gt;
    &lt;/div&gt;
  &lt;/div&gt;

  {/* Футер с очисткой */}
  &lt;div style={{ marginTop: 'auto' , paddingTop: '15px' , display: 'flex' , justifyContent: 'space-between' ,
    alignItems: 'center' }}&gt;
    &lt;span style={{ fontSize: '12px' , color: '#888' }}&gt;Всего предметов: {furniture.length}&lt;/span&gt;
    &lt;button onClick={()=&gt; useStore.setState({ furniture: [] })}
      style={{ background: '#ff6b6b', color: 'white', border: 'none', padding: '6px 12px', borderRadius: '4px', cursor:
      'pointer', fontSize: '12px' }}
      &gt;
      Очистить
    &lt;/button&gt;
  &lt;/div&gt;

&lt;/div&gt;
)
}

export default FurnitureCatalog
</code>
</pre>
  </p>
</body>

</html>
