Modalopix
===========

A modal component for React applications.

Installation
------------

You need node.js and npm. You should probably install this globally.
To install the modal component, run the following command:

**Npm way**

    npm i modalopix

Usage
-----------------------

To use the Modal component, import it into your React component and import useState:

```javascript
import {useState} from "react";
import Modal from 'modal-component';
```

Then, you can use the Modal component in your JSX like this:

```javascript
const [openModal, setOpenModal] = useState(true);

const fonctionClosebtn = () => {
	setOpenModal(false)
}

<Modal openModal={openModal} setOpenModal={setOpenModal} functionCloseBtn={functionCloseBtn}>
	{/* Modal content goes here */}
</Modal>

```

Props
------------

The modal component takes the following props:

-openModal (boolean): whether the modal is open or closed

-setOpenModal (function): a function to set the value of openModal

-functionCloseBtn (function): a function to be called when the close button is clicked



Styling
------------

The modal component comes with a default set of styles, which can be overridden by creating a modal.css file in your
project and including your own styles.


Customization
------------

The modal component can be customized by passing in your own content as children. The close button can also be
customized by replacing the cross.svg file with your own image.

