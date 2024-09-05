# Interfaz con el usuario
def interface():
    print("\nBienvenido al sistema experto.")
    symptom = input("Por favor ingrese su síntoma: ")
    
    # Tratamiento del conocimiento
    inference_engine = InferenceEngine(knowledge_base)
    explanation_module = ExplanationModule()
    
    result = inference_engine.infer(symptom)
    explanation = explanation_module.explain(result)
    
    print(explanation)

# Simulación de interacción con el usuario
interface()
