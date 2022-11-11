## Deployment Overview


## Deployment Steps

To deploy the solution manually:

1.    Download the AWS CloudFormation template from the deployment folder to your local hard drive.
2. Sign in to the <a href="https://console.aws.amazon.com/cloudformation/home" rel="noopener noreferrer" target="_blank"><span>AWS CloudFormation console</span></a>. Pre-requisites: You do not need administrator privileges, but you will need permissions to install a CloudFormation stack, and permissions to install templates in Amazon Pinpoint. 
3. Select <b>Create stack</b>.
4. On the <b>Create stack</b> page, Specify <b>template section</b>, select <b>Upload a template file</b>.
5. Under <b>Upload a template file</b>, select <b>Choose file</b> and select the template from your local drive.
6. Choose Next and follow the steps in Launch the stack below.

## Launch the stack

When you launch the stack, you are asked to provide a stack name
and parameters defined in the template (refer to matching numbers on the
image on the right as to where the parameter “appears” in the template):

<table style="width:100%">
  <tr>
    <th style="width:50%"> 
    <ol>
    <li>
        Stack Name: A Unique Stack Name is required for each Cloud Formation stack install.  We use the stack name provided to name the email templates being installed.  This allows you to install the stack multiple times if you wish (with different stack names).  This is useful when (for example) you are supporting multiple brands or companies from one Pinpoint service account, so you can customize each set of email templates for each brand with unique color schemes, company details etc
    </li>
    <li>  
        CompanyName: The name of the company or brand for this stack set of templates
    </li>
    <li>
        FooterCompanyContactDetails: Each email template has a footer with the contact details of the company.  Simply provide teh text to go into that placeholder.  e.g. company name, address and phone number. 
    </li>
    <li>
        LogoSource: The URL to the company logo / brand logo
    </li>
    <li>
        URLS for the templates: These URLs will be the target for the button click (The Call To Action) depndening on the template type. \
    </li>
    <li>
        FirstNameAttribute: The {{}} notation tag that is used for First Name in your segment data
    </li>
    <li>
        UnsubscribeMessage: The full unsbscribe message, including URL in the footer.  we default to the SES Unsubscribe URL.
    </li>
    <li>
        Theme Colors: Colors for the theme.     
    </li>
    <li>
        Template Images: We use free to use and distribute images from unsplash.com but these can be customized at install time, or after installation via the editor.
    </li>
    <ol>
    </th>
    <th>
    <img src="/deployment/example-template-screenshot-annotated.png" alt="example" >
    </th>
   </tr> 
</table>

