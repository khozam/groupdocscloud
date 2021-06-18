---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Ruby"
platform_tag: "ruby"

############################# Head ############################
head_title: "Ruby Document & Image Annotation Cloud SDK for PDF Word Excel HTML"
head_description: "Ruby Cloud SDK for managing images and document annotations. Use REST APIs to easily manipulate PDF, image, HTML, Word, Excel, & email annotation."

############################# Header ############################
title: "Let's Annotate in Ruby with RESTful API"
description: "REST API & Cloud SDK for Ruby to build online document & image annotation tools with support for text & image annotation options. Let's annotate!"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation Cloud SDK for Ruby"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-ruby.png"
        product: "GroupDocs.Annotation"
        platform: "Ruby"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/annotation/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-ruby"
        link_learn: "https://docs.groupdocs.cloud/annotation/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Cloud SDK for Ruby RESTful APIs is all you need to build document annotator tools in Ruby. Your application will be able to add annotations, watermark overlays, text replacements, redactions, sticky notes and text markups to the business documents of all popular formats such as, PDF, Microsoft Word, Excel, PowerPoint, Outlook, images other formats. Rapidly develop Annotation applications in Ruby using our SDK that works as a wrapper around Ruby APIs and makes the solution cross-platform compatible. Support for 3rd party cloud storage providers, e.g., Amazon S3, Windows Azure, Dropbox and others is also provided.‎



    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ruby Gem is required for communicating with the GroupDocs.Annotation Cloud SDK API for Ruby.‎
      
        left:
          enable: false
          icon: "fas fa-crop"
          title: "Figure Annotations"
          content: |
            
        right:
          enable: true
          icon: "fas fa-cubes"
          title: "Ruby Gem"
          content: |
            
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation Cloud SDK APIs support following file formats:‎


        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, RTF
                * **Excel**:  XLS, XLSX, XLSM, XLSB, CSV
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Visio**: VSD, VSDX, VSS, VST

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT, ODS, ODP
                * **Image Files**: BMP, PNG, JPG, JPEG, TIFF, TIF, GIF
                * **Fixed Layout**: PDF
                * **Web**: HTM, HTML
                * **Email**: EML
                * **CAD**: DWG, DXF


      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation set of SDK REST APIs is not dependent on your local operating system or ‎database. We offer our SDK APIs in numerous programming languages and with frequent new ‎additions.‎‎
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Advanced Document Annotation REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Support for Multiple File Formats"

      # feature loop
      - icon: "fas fa-desktop"
        content: "Import Annotation Information from Document & Return the List of Imported Annotations"

      # feature loop
      - icon: "fas fa-comment"
        content: "Export/Add Annotation to a Document & Retrieve the Resultant Document as Stream"
      
      # feature loop
      - icon: "fas fa-puzzle-piece"
        content: "Render Document Pages to Images and Retrieve Images’ Links"

      # feature loop
      - icon: "fas fa-retweet"
        content: "Retrieve Link to Previously Generated Image by Page Number of Annotated Document"

      # feature loop
      - icon: "fas fa-archive"
        content: "Render Document to PDF, Save Resultant Document to Storage & Fetch its Link"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render Document to PDF as an Output Stream"

      # feature loop
      - icon: "fas fa-eye-slash"
        content: "Add Text Redaction Annotation in Slides‎"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Add Annotations to Header/Footer of Microsoft Word Documents"
    
    more_feature:
      # more_feature_loop
      - title: "Easy Integration"
        content: "Integrating GroupDocs.Annotation Cloud SDK into your ruby applications is very easy. No installation is ‎required on the server or client side. Just create an account at GroupDocs.CLOUD to get App SID & ‎key. Following example shows how easy it is to import annotation information using Ruby:‎"

      # more_feature_loop
      - title: "Import Annotation Information - Ruby"
        content: |
          
          ```rb
            # TODO: Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
            # For complete examples and data files, please go to https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-ruby
                
            # Extracts annotations from document.
                def get_import
                @config = GroupDocsAnnotationCloud::Configuration.new(Utils::APP_SID, Utils::APP_KEY)
                @config.api_base_url = Utils::API_BASE_URL
                @filename = 'Annotated.pdf'
                @foldername = nil      
                
                @annotation_api = GroupDocsAnnotationCloud::AnnotationApi.from_config(@config)     
                request = GroupDocsAnnotationCloud::GetImportRequest.new(@filename,@foldername)
                
            # Extracts annotations from document.
                response = @annotation_api.get_import request
                puts response
                puts 'completed'
                end
          ```
      # more_feature_loop
      - title: "Support for Numerous Annotation Types"
        content: "Using GroupDocs.Annotation Cloud SDK for Ruby, you can work with diverse types of annotations. The ‎two basic types are; Text Annotations and Figure Annotations.‎

        While using text-based annotation, you can add text comments to selected text; highlight which text ‎should be replaced with what, hide confidential text using text redaction, highlight text with ‎strikethroughs/underlines, and add sticky notes with rich text.‎

        While working with figure annotations, you can add notes to an area highlighted with a rectangle (Area ‎Annotation), add notes to any point in the document (Point Annotation), hide confidential parts of an ‎image or text (Area Redaction), draw freehand lines and shapes (Polyline), arrows pointing to an ‎object (Pointer/Arrow), create text-based watermark overlays (Watermark), and measure the ‎distance between any objects in a document (Distance Annotation).‎"

      # more_feature_loop
      - title: "Easy Customization"
        content: "GroupDocs.Annotation Cloud SDK for Ruby is 100% tested and out of the box running. The SDK is open ‎source and has an MIT license. You can use it, and even customize it for absolutely free of charge.‎‎"
      # more_feature_loop
      - title: "Interactive API Explorer"
        content: "Using our Swagger based API explorer; you can try out GroupDocs.Annotation Cloud SDK for Ruby ‎right away in your browser. This interactive API explorer gives you information about all the resources ‎that the API offers. You can also try your desired operation by interactively providing required ‎parameters.‎"
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation Cloud Product Family also includes SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for cURL"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-curl.png"
          product: "GroupDocs.Annotation"
          platform: "cURL"
          link: "/annotation/curl/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-net.png"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for PHP"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-php.png"
          product: "GroupDocs.Annotation"
          platform: "PHP"
          link: "/annotation/php/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Python"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-python.png"
          product: "GroupDocs.Annotation"
          platform: "Python"
          link: "/annotation/python/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Ruby"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-ruby.png"
          product: "GroupDocs.Annotation"
          platform: "Ruby"
          link: "/annotation/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Node.js"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-node.png"
          product: "GroupDocs.Annotation"
          platform: "Node.js"
          link: "/annotation/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Android"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-android.png"
          product: "GroupDocs.Annotation"
          platform: "Android"
          link: "/annotation/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---