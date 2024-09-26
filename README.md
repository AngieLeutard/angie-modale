angie-modale
Description
Français
angie-modale est un composant React simple et réutilisable pour afficher des modales. Il permet d'intégrer facilement des fenêtres modales dans vos projets React en offrant des fonctionnalités comme la fermeture via la touche "Escape" et la gestion du clic en dehors de la fenêtre modale.

English
angie-modale is a simple and reusable React component for displaying modals. It allows easy integration of modal windows into your React projects, offering features like closing via the "Escape" key and managing clicks outside the modal window.

Installation
Français
Installez le package via npm :

bash
Copier le code
npm install angie-modale
English
Install the package via npm:

bash
Copier le code
npm install angie-modale
Utilisation
Français
Voici un exemple de comment utiliser angie-modale dans votre projet React :

jsx
Copier le code
import React, { useState } from 'react';
import { Modal } from 'angie-modale';
import 'angie-modale/dist/modal.css'; // Assurez-vous d'importer les styles

const App = () => {
  const [isOpen, setIsOpen] = useState(false);

  const openModal = () => setIsOpen(true);
  const closeModal = () => setIsOpen(false);

  return (
    <div>
      <button onClick={openModal}>Ouvrir la Modale</button>
      <Modal isOpen={isOpen} onClose={closeModal}>
        <h2>Contenu de la modale</h2>
        <p>Ceci est une modale réutilisable !</p>
      </Modal>
    </div>
  );
};

export default App;
English
Here’s an example of how to use angie-modale in your React project:

jsx
Copier le code
import React, { useState } from 'react';
import { Modal } from 'angie-modale';
import 'angie-modale/dist/modal.css'; // Make sure to import the styles

const App = () => {
  const [isOpen, setIsOpen] = useState(false);

  const openModal = () => setIsOpen(true);
  const closeModal = () => setIsOpen(false);

  return (
    <div>
      <button onClick={openModal}>Open Modal</button>
      <Modal isOpen={isOpen} onClose={closeModal}>
        <h2>Modal Content</h2>
        <p>This is a reusable modal!</p>
      </Modal>
    </div>
  );
};

export default App;
Props
Français
Prop	Type	Description
isOpen	boolean	Définit si la modale est ouverte ou fermée
onClose	function	Fonction appelée lorsque la modale est fermée
children	node	Contenu à afficher dans la modale
English
Prop	Type	Description
isOpen	boolean	Controls whether the modal is open or closed
onClose	function	Function to call when the modal is closed
children	node	Content to display inside the modal
Styles
Français
N'oubliez pas d'importer les styles dans votre projet en ajoutant l'import suivant dans votre fichier principal :

js
Copier le code
import 'angie-modale/dist/modal.css';
English
Don't forget to import the styles into your project by adding the following import in your main file:

js
Copier le code
import 'angie-modale/dist/modal.css';
License
MIT

