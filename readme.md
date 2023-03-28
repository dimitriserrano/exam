# I - Workbox
 
## 1) liste des fonctionnalités offertes

 - la mise en cache à l'installation
 - la mise en cache dynamique
 - différentes stratégies de gestion du cache
 - la configuration des routes 
 - la synchronisation en arrière plan 
 - notification push
 - l'app continue de fonctionner hors ligne

## 2) Méthodes de cache et utilisations possibles

 - networkFirst : à utiliser pour avoir les données les plus récentes
 - cacheFirst : à utiliser pour des données qui ne changent pas
 - cacheOnly : à utiliser pour économiser les ressources
 - networkOnly : à utiliser pour un traitement basique des données
 - staleWhileRevalidate : à utiliser pour une reponse rapide mais qui sera corriger si la données à changer

## 3) uses cases à intégrer dans le projet doctoliberal

# II - Page d'incitation à l'installation de PWA
 
## 1) Créer un composant (React / Vue / angular / HTML+CSS) pour inciter et surtout guider un utilisateur à installer la PWA (navigateur nécessaire, compatibilité du device, capacités supplémentaires, etc...)

```
import { useState } from 'react'
import reactLogo from './assets/react.svg'
import './App.css'

function App() {
  const [count, setCount] = useState(0)

  return (
    <div className="App">
      <p>
        Télécharger l'app PWA pour pouvoir consulter l'application où vous voulez même hors-ligne !! 
        Pour télécharger cliquer sur le bouton télécharger l'app.
        Sur l'application vous pourrez recevoir des notifications pour vous rappeller vos rendez vous.
        L'app est disponible sur tous les smartphones.
      </p>
      <button>Télécharger l'app</button>
    </div>
  )
}

export default App
```

## 2) Expliquer en quoi il serait interessant de mettre en place une telle page