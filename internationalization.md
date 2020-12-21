# Internationalization and localization settings
Django provides several settings for internationalization. The following settings
are the most relevant ones:
• USE_I18N: A Boolean that specifies whether Django's translation system is
enabled. This is True by default.
• USE_L10N: A Boolean indicating whether localized formatting is enabled.
When active, localized formats are used to represent dates and numbers.
This is False by default.
• USE_TZ: A Boolean that specifies whether datetimes are timezone-aware.
When you create a project with the startproject command, this is set
to True.
• LANGUAGE_CODE: The default language code for the project. This is in
standard language ID format, for example, 'en-us' for American English,
or 'en-gb' for British English. This setting requires USE_I18N to be set
to True in order to take effect. You can find a list of valid language IDs
at http://www.i18nguy.com/unicode/language-identifiers.html.
• LANGUAGES: A tuple that contains available languages for the project. They
come in two tuples of a language code and language name. You can see the
list of available languages at django.conf.global_settings. When you
choose which languages your site will be available in, you set LANGUAGES
to a subset of that list.
• LOCALE_PATHS: A list of directories where Django looks for message files
containing translations for the project.
• TIME_ZONE: A string that represents the timezone for the project. This is set
to 'UTC' when you create a new project using the startproject command.
You can set it to any other timezone, such as 'Europe/Madrid'.