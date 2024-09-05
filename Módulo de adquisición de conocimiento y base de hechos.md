# Módulo de adquisición de conocimiento alimentando la base de conocimientos
knowledge_base = KnowledgeBase()

# Agregamos hechos y reglas del conocimiento
for symptom, treatment in expert_knowledge.items():
    knowledge_base.add_rule(f"Si el paciente tiene {symptom}, {treatment}")
    
for sensor, value in sensor_data.items():
    knowledge_base.add_fact(f"El sensor detecta {sensor} con valor {value}")

print("\nBase de Conocimientos - Reglas:")
for rule in knowledge_base.get_rules():
    print(rule)

print("\nBase de Hechos:")
for fact in knowledge_base.get_facts():
    print(fact)
