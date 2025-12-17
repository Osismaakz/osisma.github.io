import React, { useState } from 'react';

import { Calendar, Clock, Phone, Mail, MapPin, User, CalendarDays, MessageCircle, CheckCircle } from 'lucide-react';

 

const App = () => {  

  const [formData, setFormData] = useState({

    childName: '',

    parentName: '',

    age: '',

    phone: '',

    email: '',

    date: '',

    time: '',

    message: ''

  });

 

  const [submitted, setSubmitted] = useState(false);

 

  const handleChange = (e) => {

    setFormData({

      ...formData,

      [e.target.name]: e.target.value

    });

  };
