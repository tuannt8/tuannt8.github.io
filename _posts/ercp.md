
# ERCP procedure

ERCP stands for Endoscopic Retrograde Cholangiopancreatography. This is a medical procedure that combines upper gastrointestinal (GI) endoscopy and X-rays to treat problem of bile duct and pancreatic duct. More information can be found at [What is ERCP][ERCP].

I research on a simulation of sphincterotomy, a procedure in ERCP. In this procedure, doctor use sphincterotome device to cut and enlarge major papilla of duodenum for cannulation.

{% include image-caption.html img="/img/ERCP-illu.jpg" caption="Inserting endoscope to patient duodenum" alt="paper-demo" imgsource="http://www.hopkinsmedicine.org/liver_tumor_center/conditions/bile_duct_cancer.html" %}

# ERCP simulation

Simulation of sphincterotomy is being developed. We employ meshfree method to model soft tissue and develop a contact model and a cutting algorithm.

A real-time simulation is shown in the demonstration video. The simulation provides high fidelity in compared with real procedure (captured image).

<div class="row">
<div class="large-6 medium-6 columns" markdown="1">

{% include image-caption.html img="/img/real-sphinc.png" caption="Real image captured from ERCP video (Provided by Woman Medical Center, Korea)" alt="paper-demo" %}

</div><div class="large-6 medium-6 columns" markdown="1">

{% include youtube.html src="http://www.youtube.com/embed/YkOgbarneHE"  width="280" height="280"  
caption="Video demonstration of sphincterotomy" %}

</div>
</div>

[ERCP]:http://www.niddk.nih.gov/health-information/health-topics/diagnostic-tests/ercp/Pages/diagnostic-test.aspx